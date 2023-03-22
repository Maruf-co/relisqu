<script lang="ts">
  interface CommonJoke {
    alt: string;
    day: string;
    month: string;
    year: string;
    img: string;
    title: string;
  }

  interface SingleJoke extends CommonJoke {
    type: "single";
    joke: string;
  }

  interface TwopartJoke extends CommonJoke {
    type: "twopart";
    setup: string;
    delivery: string;
  }

  type Joke = SingleJoke | TwopartJoke;

  const myEmail: string = "m.asatullaev@innopolis.university";

  const jokeImage = {
    alt: '',
    src: '/'
  }
  let jokeTitle: string = "Wait, I'm thinking...";

  let jokeDate: string;
  

  const getId = async (email: string): Promise<string> => {
    const id: string = await fetch(
      `https://fwd.innopolis.app/api/hw2?email=${email}`
    ).then((res) => res.json());

    return id;
  };

  const fetchJoke = async (id: string): Promise<Joke> => {
    const jokeResponse: Joke = await fetch(
      `https://getxkcd.vercel.app/api/comic?num=${id}`
    ).then((res) => res.json());

    return jokeResponse;
  };

  const fillJokeObject = (jokeObj: Joke) => {
    const { alt, title, img, year, month, day } = jokeObj;

    const date: Date = new Date(
      parseInt(year),
      parseInt(month) - 1,
      parseInt(day)
    );

    jokeImage.src = img;
    jokeImage.alt = alt;
    jokeTitle = title;
    jokeDate = date.toLocaleDateString();
  };

  const showJoke = async () => {
    const jokeId = await getId(myEmail);

    const jokeObj: Joke = await fetchJoke(jokeId);

    fillJokeObject(jokeObj);
  };

  showJoke();
</script>

<div class="jokeBody">
  <h1 class="jokeTitle">{jokeTitle}</h1>
  <img class="jokeImage" alt={jokeImage.alt} src={jokeImage.src} />
  <p class="jokeDate">{jokeDate}</p>
</div>

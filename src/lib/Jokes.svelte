<script lang="ts">
  import TitleWithImage from "./TitleWithImage.svelte";
  import JokesFromServer from "./JokesFromServer.svelte";
  const avatar = 'https://github.com/Maruf-co/Portfolio/blob/main/src/content/avatar.png?raw=true';
</script>

<section id="jokes">
  <hr class="divideLine" />
  
  <TitleWithImage
    img={{ alt: "Avatar", src: avatar }}
    title={"I also like jokes, lol kek<br />Check it out below"}
  />

  <JokesFromServer />
</section>

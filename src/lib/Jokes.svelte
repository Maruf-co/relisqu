<script lang="ts">
  import TitleWithImage from "./TitleWithImage.svelte";
  import JokesFromServer from "./JokesFromServer.svelte";
  import avatar from "$lib/assets/avatar.png";
</script>

<section id="jokes">
  <hr class="divideLine" />
  
  <TitleWithImage
    img={{ alt: "Avatar", src: avatar }}
    title={"I also like jokes, lol kek<br />Check it out below"}
  />

  <JokesFromServer />
</section>

<script lang="ts">
  import TitleWithImage from "./TitleWithImage.svelte";

  import JokesFromServer from "./JokesFromServer.svelte"
</script>

<section id="jokes">
  <hr class="divideLine" />
  
  <TitleWithImage
    img={{ alt: "Avatar", src: "/avatar.png" }}
    title={"I also like jokes, lol kek<br />Check it out below"}
  />

  <JokesFromServer />
</section>

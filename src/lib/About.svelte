<script lang="ts">
  import TitleWithImage from "$lib/TitleWithImage.svelte";
  import avatar from "$lib/assets/avatar.png";
</script>


<section id="about">
  <hr class="divideLine" />
  <TitleWithImage
    img={{ alt: "Avatar", src: avatar }}
    title={"Hello, I'm Anna.<br />I'm a game developer<br />and an artist."}
  />
  
  <p class="bio">
    I have 2 years of experience in game development.
    <br />
    And 6 years in art, especially in pixel art.
  </p>
</section>

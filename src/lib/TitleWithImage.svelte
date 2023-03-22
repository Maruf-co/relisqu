<script lang="ts">
    export let img: {
        alt: string;
        src: string;
    };
    export let title: string;
</script>


<div class="titleWithImage">
  <img class="authorImage" alt={img.alt} src={img.src} />
  <h1 class="title">
    {@html title}
  </h1>
</div>
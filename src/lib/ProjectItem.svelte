<script lang="ts">
  export let title: string;
  export let description: string;
  export let video: {
    width: string;
    height: string;
    src: string;
  };
</script>

<li class="project">
  <div class="descrBlock">
    <h3>{title}</h3>
    <p class="decription">
      {@html description}
    </p>
  </div>
  <video
    class="gif"
    width={video.width}
    height={video.height}
    autoplay
    loop
    muted
  >
    <source src={video.src} type="video/mp4" />
    Your browser does not support the video tag Т-Т
  </video>
</li>

<script lang="ts">
  export let link: {
    id: string;
    href: string;
  };
  export let img: {
    alt: string;
    src: string;
  };
</script>

<li class="contact">
  <a id={link.id} href={link.href}>
    <img src={img.src} alt={img.alt} class="contactIcon" />
  </a>
</li>

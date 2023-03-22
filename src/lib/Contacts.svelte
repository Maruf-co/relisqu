<script lang="ts">
  import ContactItem from "./ContactItem.svelte";
  import mail from "$lib/assets/contactIcons/mail.svg";
  import itchIo from "$lib/assets/contactIcons/itchIo.svg";
  import telegram from "$lib/assets/contactIcons/telegram.svg";
  import github from "$lib/assets/contactIcons/github.svg";
  import twitter from "$lib/assets/contactIcons/twitter.svg";

</script>

<section id="contacts">
  <hr class="divideLine" />
  <h2 class="contactsTitle">My contacts</h2>
  <ul class="contacts">
    <ContactItem
      link={{
        id: "email",
        href: "mailto:relisqu@gmail.com",
      }}
      img={{
        alt: "mail",
        src: mail,
      }}
    />

    <ContactItem
      link={{
        id: "",
        href: "https://relisqu.itch.io/",
      }}
      img={{
        alt: "itch-io",
        src: itchIo,
      }}
    />
    <ContactItem
      link={{
        id: "tg-link",
        href: "https://t.me/relisqu_dev",
      }}
      img={{
        alt: "telegram",
        src: telegram,
      }}
    />

    <ContactItem
      link={{
        id: "gh-link",
        href: "https://github.com/relisqu",
      }}
      img={{
        alt: "github",
        src: github,
      }}
    />
    <ContactItem
      link={{
        id: "",
        href: "https://twitter.com/relisqu",
      }}
      img={{
        alt: "twitter",
        src: twitter,
      }}
    />
  </ul>
</section>

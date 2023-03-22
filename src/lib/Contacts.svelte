<script lang="ts">
  import ContactItem from "./ContactItem.svelte";
  const mail = 'https://raw.githubusercontent.com/Maruf-co/Portfolio/88ef5d7803ced56ed3235f411b41b4fbbbeed0d8/src/content/contactIcons/github.svg';
  const itchIo = 'https://raw.githubusercontent.com/Maruf-co/Portfolio/88ef5d7803ced56ed3235f411b41b4fbbbeed0d8/src/content/contactIcons/github.svg';
  const telegram = 'https://raw.githubusercontent.com/Maruf-co/Portfolio/88ef5d7803ced56ed3235f411b41b4fbbbeed0d8/src/content/contactIcons/telegram.svg';
  const github = 'https://raw.githubusercontent.com/Maruf-co/Portfolio/88ef5d7803ced56ed3235f411b41b4fbbbeed0d8/src/content/contactIcons/github.svg';
  const twitter = 'https://raw.githubusercontent.com/Maruf-co/Portfolio/88ef5d7803ced56ed3235f411b41b4fbbbeed0d8/src/content/contactIcons/github.svg';

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

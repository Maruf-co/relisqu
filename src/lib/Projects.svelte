<script lang="ts">
  import ProjectItem from "./ProjectItem.svelte";
  const hookYou = "https://github.com/Maruf-co/Portfolio/blob/main/src/content/projects/hookYou.mp4?raw=true";
  const mouse = "https://github.com/Maruf-co/Portfolio/blob/main/src/content/projects/mouse.mp4?raw=true";
  const pingPong = "https://github.com/Maruf-co/Portfolio/blob/main/src/content/projects/pingPong.mp4?raw=true";
  const anlaut = "https://github.com/Maruf-co/Portfolio/blob/main/src/content/projects/anlaut.mp4?raw=true";

</script>

<section id="projects">
  <hr class="divideLine" />
  <ul class="projectsWrap">
    <ProjectItem
      title={"Hook you"}
      description={"Game where you playing as some kind of fox with hook that is have to go to the next room. Game is full of interesting and aesthetic details.<a class='link' href='https://relisqu.itch.io/hookyou'>check it out</a>"}
      video={{
        width: "352",
        height: "334",
        src: hookYou,
      }}
    />
    <ProjectItem
      title={"BringSnowball"}
      description={"Here you are a litsle mouse whose mission is to bring snow ball to the specific spot going through different obstacles. But snowball is melting, so hurry up!"}
      video={{
        width: "320",
        height: "172",
        src: mouse,
      }}
    />
    <ProjectItem
      title={"Space Ping Pong"}
      description={"Classic very popular ping pong game where you have to move platform, to bounce the ball that breaks the bricks. Be careful and don't break lost your ball :)"}
      video={{
        width: "362",
        height: "300",
        src: pingPong,
      }}
    />
    <ProjectItem
      title={"Anlaut"}
      description={"Game which is some kind of add-on over classic flappy bird game. You could take some more species with yourself that gives you extralives and have unique properties such as blasters to shout the enemies. Mission is to go as far as you can or go till the end of the level."}
      video={{
        width: "198",
        height: "358",
        src: anlaut,
      }}
    />
  </ul>
</section>

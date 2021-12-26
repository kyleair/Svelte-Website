<script>
  import Icon from "svelte-awesome";
  import {
    linkedinSquare,
    envelope,
    twitter,
    github,
  } from "svelte-awesome/icons";
</script>

<main>
  <h1 id="socials">
    <span id="anchor" />Socials
    <img alt="" src="./assets/socialicon.png" height="50px" weight="50px" />
  </h1>

  <h2>
    If you'd like to get in touch you can reach out over LinkedIn, Email
    (kyleair8@gmail.com) or Twitter!
  </h2>
  <a href="https://www.linkedin.com/in/kyle-air-813853164/" target="_blank"
    ><Icon data={linkedinSquare} scale="4" /></a
  >
  <a href="mailto:kyleair8@gmail.com" target="_blank" class="iconThingy"
    ><Icon data={envelope} scale="4" /></a
  >
  <a href="https://twitter.com/riaelyk" target="_blank"
    ><Icon data={twitter} scale="4" /></a
  >
  <a href="https://github.com/kyleair/Svelte-Website" target="_blank"
    ><Icon data={github} scale="4" /></a
  >
</main>

<style>
  a {
    padding: 3% 6%;
  }
  main {
    padding-bottom: 5vh;
  }
  h2 {
    padding: 0 0 3%;
  }
  .iconThingy {
    color: black;
  }
  .iconThingy:hover {
    opacity: 0.35;
  }
</style>

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
    <img alt="" src="./assets/socialicon.png" height="48px" weight="48px" />
  </h1>
  <h2>
    Check out my <a
      href="./content/Kyle_Air_Resume.pdf"
      target="_blank"
      class="resume">resume</a
    >. Feel free to download it and contact me if you have any questions!
  </h2>
  <h2>
    If you'd like to get in touch you can reach out over LinkedIn, Email
    (kyleair8@gmail.com) or Twitter!
  </h2>
  <a
    href="https://www.linkedin.com/in/kyle-air-813853164/"
    target="_blank"
    rel="noopener noreferrer"
    class="iconThingy"
    ><Icon data={linkedinSquare} scale="4" label="linkedin" /></a
  >
  <a href="mailto:kyleair8@gmail.com" target="_blank" class="iconThingy"
    ><Icon data={envelope} scale="4" label="email" /></a
  >
  <a
    href="https://twitter.com/riaelyk"
    target="_blank"
    rel="noopener noreferrer"
    class="iconThingy"><Icon data={twitter} scale="4" label="tiwtter" /></a
  >
  <a
    href="https://github.com/kyleair/Svelte-Website"
    target="_blank"
    rel="noopener noreferrer"
    class="iconThingy"><Icon data={github} scale="4" label="github" /></a
  >
</main>

<style>
  a {
    padding: 3% 6%;
  }
  a.resume {
    padding: 0;
    color: blue;
    text-decoration: underline;
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

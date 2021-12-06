<script>
  import SocialIcons from "@rodneylab/svelte-social-icons";
</script>

<main>
  <h1 id="socials">
    <span id="anchor" />Socials
    <img alt="" src="./assets/socialicon.png" height="50px" weight="50px" />
  </h1>

  <h2>
    If you'd like to get in touch you can reach out over LinkedIn, Email or
    Twitter!
  </h2>
  <a href="https://www.linkedin.com/in/kyle-air-813853164/" target="_blank"
    ><SocialIcons alt="" network="linkedin" fgColor="#ffffff" /></a
  >
  <a href="mailto:kyleair8@gmail.com" target="_blank"
    ><SocialIcons alt="" network="email" fgColor="#ffffff" /></a
  >
  <a href="https://twitter.com/riaelyk" target="_blank"
    ><SocialIcons alt="" network="twitter" fgColor="#ffffff" /></a
  >
  <a href="https://github.com/kyleair/Svelte-Website" target="_blank"
    ><SocialIcons alt="" network="github" fgColor="#ffffff" /></a
  >
</main>

<style>
  a {
    padding: 3% 6%;
  }
  main {
    padding-bottom: 5vh;
  }
</style>

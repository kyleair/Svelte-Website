<script>
  import About from "./components/aboutme.svelte";
  import Experience from "./components/experience.svelte";
  import Education from "./components/education.svelte";
  import Socials from "./components/socials.svelte";
  import Navbar from "./components/navibar.svelte";
  import Projects from "./components/projects.svelte";
</script>

<html lang="en">
  <div class="container">
    <Navbar />
    <div class="content">
      <About />
      <Experience />
      <Education />
      <Projects />
      <Socials />
    </div>
  </div>
</html>

<style>
  .content {
    text-align: center;
    margin-left: 20%;
    margin-right: 20%;
    padding-top: 5%;
  }
  html {
    background-color: #f9f4f4;
  }
</style>

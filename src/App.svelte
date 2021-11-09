<script>
  import About from "./components/aboutme.svelte";
  import Experience from "./components/experience.svelte";
  import Education from "./components/education.svelte";
  import Socials from "./components/socials.svelte";
  import Navbar from "./components/navibar.svelte";
  import Projects from "./components/projects.svelte";
</script>

<Navbar />
<main>
  <About />
  <Experience />
  <Education />
  <Projects />
  <Socials />
</main>

<style>
  main {
    text-align: center;
    margin-left: 20%;
    margin-right: 20%;
    padding-top: 5%;
  }
</style>

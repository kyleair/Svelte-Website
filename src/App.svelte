<script>
  import About from "./components/aboutme.svelte";
  import Experience from "./components/experience.svelte";
  import Education from "./components/education.svelte";
  import Socials from "./components/socials.svelte";
  import Navbar from "./components/navibar.svelte";
  import Projects from "./components/projects.svelte";
  import Modal from "svelte-simple-modal";
</script>

<html lang="en">
  <Modal>
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
  </Modal>
</html>

<style>
  .content {
    text-align: center;
    margin-left: 20%;
    margin-right: 20%;
    padding-top: 4%;
  }
  @media screen and (max-width: 1800px) {
    .content {
      margin-left: 10%;
      margin-right: 10%;
    }
  }
</style>

<script>
  import projects from "../../public/content/projectcontent";
  import SocialIcons from "@rodneylab/svelte-social-icons";
  import projectmodal from "./modals/projectmodal.svelte";

  import { getContext } from "svelte";

  const { open } = getContext("simple-modal");

  const showProject = () => {
    open(projectmodal, {});
  };
</script>

<main>
  <h1 id="projects"><span id="anchor" />Projects 💻</h1>
  <div class="projects-area">
    {#each projects as project}
      <div class="project-block tile-hover" on:click={() => showProject()}>
        <div class="text-container">
          <h2>
            {project.name}
          </h2>
          <p>{project.shortDescription}</p>
          <a href="https://github.com/kyleair/Svelte-Website" target="_blank"
            ><SocialIcons
              alt=""
              network="github"
              fgColor="#ffffff"
              width="30"
              height="30"
            /></a
          >
        </div>
        <div class="img-container">
          <img alt="picting" src={project.img} width="95%" height="95%" />
        </div>
      </div>
    {/each}
  </div>
</main>

<style>
  .projects-area {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: auto auto;
    margin-bottom: 15px;
    gap: 1px 1px;
  }
  .project-block {
    display: grid;
    grid-template-rows: auto auto;
    row-gap: 1.5vh;
    border-color: black;
    border-style: solid;
    border-width: 1px;
    border-radius: 50px;
    margin: 20px;
    padding: 10px;
    background-color: rgb(176, 224, 230, 0.3);
  }
  .text-container {
    margin: auto;
  }
  .img-container {
    border-top: dashed black 1px;
    background-image: url("./assets/betappthreescreens.png");
  }
  img {
    object-fit: scale-down;
  }
  p {
    text-align: center;
    margin: 0.7rem 1rem;
  }
</style>

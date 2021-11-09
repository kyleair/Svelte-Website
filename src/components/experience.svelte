<script>
  import experiences from "../../public/content/experiencecontent";
</script>

<main>
  <h1 id="experience"><span id="anchor" />Experience 👔</h1>
  <div class="experience-area">
    {#each experiences as experience}
      <div class="experience-block">
        <h2>{experience.company}</h2>
        <h3>{experience.title}</h3>
        <h4>{experience.timeStarted} - {experience.timeEnded}</h4>
        <p>{experience.shortDescription}</p>
      </div>
    {/each}
  </div>
</main>

<style>
  .experience-area {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: auto auto;
    margin-bottom: 15px;
    gap: 1px 1px;
    grid-template-areas: "experienceitem";
  }
  .experience-block {
    border-color: black;
    border-style: solid;
    border-width: 3px;
    border-radius: 50px;
    margin: 20px;
    padding: 10px;
    background-color: lightcyan;
  }
</style>

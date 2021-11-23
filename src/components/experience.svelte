<script>
  import experiences from "../../public/content/experiencecontent";
  import experiencemodal from "./modals/experiencemodal.svelte";
  import { getContext } from "svelte";

  const { open } = getContext("simple-modal");

  const showExperience = (
    title,
    link,
    company,
    start,
    end,
    description,
    location
  ) => {
    open(experiencemodal, {
      title: title,
      link: link,
      company: company,
      start: start,
      end: end,
      description: description,
      location: location,
    });
  };
</script>

<main>
  <h1 id="experience"><span id="anchor" />Experience 👔</h1>
  <div class="experience-area">
    {#each experiences as experience}
      <div
        class="experience-block tile-hover"
        on:click={() =>
          showExperience(
            experience.title,
            experience.link,
            experience.company,
            experience.timeStarted,
            experience.timeEnded,
            experience.shortDescription,
            experience.location
          )}
      >
        <div>
          <h2>
            {experience.company}
          </h2>
          <h3>{experience.title}</h3>
          <h4>{experience.timeStarted} - {experience.timeEnded}</h4>
          <p>{experience.shortDescription}</p>
        </div>
        <div class="seperator" />
        <div class="img-container">
          <img
            alt="picting"
            src={experience.imgPath}
            height={experience.imgHeight}
            width={experience.imgWidth}
          />
        </div>
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
  }
  .experience-block {
    display: grid;
    grid-template-columns: 7fr 2fr 3fr;
    grid-gap: 0px;
    border-color: black;
    border-style: solid;
    border-width: 1px;
    border-radius: 50px;
    margin: 20px;
    padding: 10px;
    background-color: rgb(176, 224, 230, 0.3);
    position: relative;
    z-index: 1;
  }
  .img-container {
    align-self: center;
    justify-self: center;
  }
  .seperator {
    align-self: center;
    justify-self: center;
    border-left: 1px solid black;
    height: 7rem;
  }
  p {
    text-align: center;
    margin: 0.5rem 1rem;
  }
</style>

<script>
  import experiences from "../../public/content/experiencecontent";
</script>

<main>
  <h1 id="experience"><span id="anchor" />Experience 👔</h1>
  <div class="experience-area">
    {#each experiences as experience}
      <div class="experience-block">
        <div>
          <h2>
            <a href={experience.link} target="_blank"> {experience.company}</a>
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

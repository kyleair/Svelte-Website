<script>
  import educationmodal from "./modals/educationmodal.svelte";
  import { getContext } from "svelte";

  const { open } = getContext("simple-modal");

  const showEducation = () => {
    open(
      educationmodal,
      {},
      {
        styleWindow: { backgroundColor: "#d4fffc" },
      }
    );
  };
</script>

<main>
  <h1 id="education">
    <span id="anchor" />Education
    <img alt="" src="./assets/educationicon.png" height="50px" weight="50px" />
  </h1>
  <div class="education-block tile-hover" on:click={() => showEducation()}>
    <div>
      <h2>Queen's University</h2>
      <h3>Applied Mathematics and Computer Engineering</h3>
      <h4>Class of 2021</h4>
    </div>
    <div class="seperator" />
    <div class="img-container">
      <img alt="picting" src="./assets/Queens.png" height="99" width="130" />
    </div>
  </div>
</main>

<style>
  .education-block {
    display: grid;
    grid-template-columns: 6fr 2fr 3fr;
    grid-gap: 0px;
    border-color: black;
    border-style: solid;
    border-width: 1px;
    border-radius: 50px;
    background-color: #ffecb5;
    margin: auto;
    padding: 10px;
    width: 38vw;
  }
  .seperator {
    align-self: center;
    justify-self: center;
    border-left: 1px solid black;
    height: 7rem;
  }
  .img-container {
    align-self: center;
    justify-self: center;
    margin-right: 3rem;
  }
  @media screen and (max-width: 1000px) {
    .education-block {
      width: 80vw;
    }
  }
  @media screen and (max-width: 600px) {
    .education-block {
      grid-template-columns: 1fr 0fr 0fr;
    }
    .seperator,
    .img-container {
      display: none;
    }
  }
</style>

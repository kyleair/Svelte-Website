<script>
  import Icon from "svelte-awesome";
  import { code } from "svelte-awesome/icons";

  export let title;
  export let description;
  export let imgPath;
  export let github;
</script>

<main>
  <h1>{title}</h1>
  <a href={github} target="_blank"><Icon data={code} scale="2" /></a>
  <p>{description}</p>
  <a href={imgPath} target="_blank"
    ><img
      alt="Project"
      src={imgPath}
      style="width:45%;height:auto;max-width:45vw"
    /></a
  >
</main>

<style>
  main,
  main h1,
  main p,
  main img {
    text-align: center;
  }
  p {
    border: dashed black;
    border-width: 0 0 1px;
    padding: 1em 10% 3em;
    margin: auto auto;
  }
  img {
    margin: 2em;
    border: solid black 1px;
  }
  img:hover {
    border: solid black 2px;
    -webkit-transition-duration: 0.3s;
    transition-duration: 0.3s;
    -webkit-transform: scale(1.05);
    transform: scale(1.05);
  }
</style>

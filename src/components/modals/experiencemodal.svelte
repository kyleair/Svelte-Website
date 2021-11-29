<script>
  export let title;
  export let link;
  export let company;
  export let start;
  export let end;
  export let description;
  export let location;
</script>

<main>
  <div class="header">
    <h2>
      {title}
    </h2>
    <p>for</p>
    <h2>
      <a href={link} target="_blank" class="company-link">{company}</a>
    </h2>
  </div>
  <div class="datelocation">
    <h3 class="date">{start} - {end}</h3>
    <h3 class="location">{location}</h3>
  </div>
  <ul>
    {#each description as desc}
      <li>{desc}</li>
    {/each}
  </ul>
</main>

<style>
  .company-link {
    color: blue;
  }
  .company-link:hover {
    text-decoration: underline;
    color: rgb(0, 0, 0, 0.4);
  }
  h2,
  p {
    display: inline;
  }
  .header p {
    font-size: larger;
    padding: 0 0.1em;
  }
  h2 {
    font-size: x-large;
  }
  p {
    padding: 0 1em;
  }
  .header {
    padding-bottom: 20px;
    border-bottom: solid black 1px;
    text-align: center;
  }
  .datelocation {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  .date {
    text-align: left;
    padding-left: 1em;
  }
  .location {
    text-align: right;
    padding-right: 1em;
  }
</style>

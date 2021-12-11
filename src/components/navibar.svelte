<script>
</script>

<div class="bar">
  <div class="grid-container">
    <div class="homebuttonwrapper">
      <a href="/"
        ><img
          alt="Home"
          src="./assets/homebutton.png"
          height="40px"
          weight="40px"
        /></a
      >
    </div>
    <div class="namewrapper"><h1>Kyle Air</h1></div>
    <div class="sectionwrapper">
      <a href="#about"><h2>About Me</h2></a>
      <h3>&#183;</h3>
      <a href="#experience"><h2>Experience</h2></a>
      <h3>&#183;</h3>
      <a href="#education"><h2>Education</h2></a>
      <h3>&#183;</h3>
      <a href="#projects"><h2>Projects</h2></a>
      <h3>&#183;</h3>
      <a href="#socials"><h2>Socials</h2></a>
    </div>
  </div>
</div>

<style>
  .bar {
    border-style: solid;
    border-bottom-color: black;
    border-width: 0px;
    border-bottom-width: 1px;
    position: fixed;
    z-index: 999;
    left: 0;
    top: 0;
    width: 100%;
    height: 4.5em;
    background-image: linear-gradient(to right, #ffecb5, #ffe59c);
    justify-content: center;
  }
  a {
    padding: 1%;
  }
  .sectionwrapper {
    display: flex;
    justify-content: right;
    align-items: center;
  }
  .homebuttonwrapper {
    display: flex;
    justify-content: left;
  }
  .namewrapper {
    display: flex;
    justify-content: center;
    border: solid black;
    border-width: 0px 1px;
  }
  .grid-container {
    display: grid;
    grid-template-columns: 1fr 3fr 6fr;
    align-items: center;
    margin-left: 20%;
    margin-right: 20%;
  }
  h1 {
    border: none;
    padding: 0;
    margin: auto;
  }
  @media screen and (max-height: 600px) {
    .bar {
      visibility: hidden;
    }
  }
</style>

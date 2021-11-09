<script>
</script>

<div class="bar">
  <div class="grid-container">
    <div class="homebuttonwrapper">
      <a href="/"
        ><img
          alt="Home"
          src="./assets/homeicon.png"
          height="40px"
          weight="40px"
        /></a
      >
    </div>
    <div class="sectionwrapper">
      <a href="#about"><h2>About Me</h2></a>
      <a href="#experience"><h2>Experience</h2></a>
      <a href="#education"><h2>Education</h2></a>
      <a href="#projects"><h2>Projects</h2></a>
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
    left: 0;
    top: 0;
    width: 100%;
    height: 10%;
    background-color: rgb(175, 250, 242);
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
  .grid-container {
    display: grid;
    grid-template-columns: 1fr 6fr;
    align-items: center;
    margin-left: 20%;
    margin-right: 20%;
  }
</style>

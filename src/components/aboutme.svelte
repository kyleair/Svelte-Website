<script>
</script>

<main>
  <h1 id="about">
    <span id="anchor" />About Me
    <img alt="" src="./assets/aboutmeicon.png" height="50px" weight="50px" />
  </h1>
  <div class="grid-container">
    <div>
      <p>
        Hello! My name is Kyle Air and I am a new graduate Software Developer
        with a passion for technology, programming, hiking, sports and video
        games. I graduated from Queen's University in 2021 with a degree in
        Engineering.
      </p>
      <p>
        I made this website to talk about myself, showcase projects I have made
        and further my own web development skills. Feel free to contact me via
        my social links at the bottom of this page, I am eager to hear any
        feedback or critique on this website and I am always open to chat.
        Thanks for stopping by!
      </p>
    </div>
    <div class="imgcontainer">
      <a href="./assets/natureheadshot1square.JPG" target="_blank"
        ><img
          class="headshot"
          alt="headshot"
          src="./assets/natureheadshot1square.JPG"
          height="200"
          width="200"
        /></a
      >
    </div>
  </div>
</main>

<style>
  .grid-container {
    display: grid;
    grid-template-columns: 2fr 1fr;
    align-items: center;
    justify-items: center;
  }
  p {
    text-indent: 4%;
    font-size: large;
  }
  img.headshot {
    border: solid rgb(0, 0, 0, 0.75) 1px;
    border-radius: 50%;
  }
  .headshot:hover {
    -webkit-transition-duration: 0.3s;
    transition-duration: 0.3s;
    -webkit-transform: scale(1.08);
    transform: scale(1.08);
  }
  @media screen and (max-width: 1000px) {
    .grid-container {
      display: flex;
      align-items: center;
      justify-items: center;
    }
  }
</style>

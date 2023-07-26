<script>
  const skills = ["SwiftUI", "Flutter", "JavaScript", "Python", "Svelte"];
</script>

<section id="about" class="main">
  <div class="row">
    <h1>About Me</h1>
    <div class="line" />
  </div>

  <div class="row space">
    <img src="avatar.png" alt="Brendan" />
    <div>
      <p>
        I am passionate about creating front-end web and mobile applications. I
        am currently seeking a full time software engineering role beginning
        summer 2024.
      </p>
      <p>
        Aside from development I am a member of the Ohio State Cheerleading team
        where I will help the program attempt to claim its' 4th UCA national
        championship. I am also an avid disc golfer.
      </p>
    </div>
  </div>

  <div class="row">
    <div class="line2" />
    <h2>Skills</h2>
  </div>

  <div class="skillRow">
    {#each skills as skill}
      <div class="skill">
        <h3 class="symbolL">&lt;</h3>
        <h3>{skill}</h3>
        <h3 class="symbolM">/</h3>
        <h3 class="symbolR">&gt;</h3>
      </div>
    {/each}
  </div>
</section>

<style>
  .main {
    margin-left: 15vw;
    margin-right: 15vw;
    height: 100vh;
  }
  img {
    width: 23.5vw;
    height: 52.5vh;
  }
  .row {
    display: flex;
    align-items: center;
  }
  h1 {
    color: white;
    font-family: Montserrat;
    font-size: 4.15vw;
    margin-top: 1.3vh;
    margin-bottom: 1.3vh;
    margin-right: 1.2vw;
  }
  p {
    color: white;
    opacity: 90%;
    font-family: Montserrat;
    font-size: 1.6vw;
    margin-top: 0;
    width: 38vw;
    line-height: 5.5vh;
  }
  .line {
    width: 67%;
    height: 0.25vh;
    background-color: #f77909;
  }
  .space {
    justify-content: space-between;
  }
  h2 {
    color: white;
    font-family: Montserrat;
    font-size: 3.1vw;
    margin-bottom: 0;
  }
  h3 {
    color: white;
    font-family: Montserrat;
    font-size: 1.55vw;
    line-height: 1.1vh;
  }
  .symbolL {
    color: white;
    opacity: 75%;
    margin-right: 0.5vw;
  }
  .symbolM {
    color: #f77909;
    margin-left: 0.5vw;
  }
  .symbolR {
    color: white;
    opacity: 75%;
    margin-left: 0.5vw;
  }
  .skill {
    display: flex;
  }
  .skillRow {
    display: flex;
    justify-content: space-between;
  }
  .line2 {
    width: 100%;
    height: 0.25vh;
    margin-right: 1.2vw;
    background-color: #f77909;
    margin-top: 5.4vh;
  }
  .skill:hover {
    transform: translateY(-1.1vh);
  }
</style>

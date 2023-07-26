<script>
  import Icon from "@iconify/svelte";
  export let inNavMode;
</script>

<section id="home" class="main">
  <div class="wrapper" on:click={() => (inNavMode = true)}>
    <Icon class="icon" icon="ri:menu-5-fill" color="white" height="28" />
  </div>
  <div class="col">
    <div class="textBox">
      <h2>Hello, my name is</h2>
      <h1>Brendan Gass</h1>
      <h3>
        I am a graduating senior studying computer science and engineering at
        the Ohio State University.
      </h3>
    </div>
  </div>
</section>

<style>
  .main {
    min-height: 100vh;
  }
  .col {
    display: flex;
    height: 85vh;
    align-items: center;
  }
  .wrapper {
    width: 28px;
    height: 28px;
    margin-top: 3.7vh;
    margin-left: 84.5vw;
  }
  h1 {
    color: white;
    font-family: Montserrat;
    font-size: 10vw;
    text-align: center;
    margin-top: 0.6vh;
    margin-bottom: 0.6vh;
  }
  h2 {
    color: #f77909;
    font-family: Montserrat;
    font-size: 3.7vw;
    margin-left: 14vw;
    margin-bottom: 0;
  }
  h3 {
    color: white;
    opacity: 75%;
    font-family: Montserrat;
    font-size: 3.7vw;
    text-align: center;
    margin-left: 14vw;
    margin-right: 14vw;
    margin-top: 0;
  }
</style>

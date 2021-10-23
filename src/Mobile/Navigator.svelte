<script>
  import Icon from "@iconify/svelte";
  export let inNavMode;
</script>

<div class="bg">
  <div class="wrapper" on:click={() => (inNavMode = false)}>
    <Icon icon="ri:close-fill" color="black" height="28" />
  </div>
  <div class="nav">
    <a href="#about"><h1 on:click={() => (inNavMode = false)}>ABOUT</h1></a>
    <a href="#projects">
      <h1 on:click={() => (inNavMode = false)}>PROJECTS</h1>
    </a>
    <a href="#contact">
      <h1 on:click={() => (inNavMode = false)}>CONTACT</h1>
    </a>

    <div class="iconRow">
      <a href="https://github.com/bgass10" target="_blank"
        ><Icon icon="simple-icons:github" color="black" height="28" /></a
      >
      <a href="https://www.linkedin.com/in/brendangass/" target="_blank">
        <Icon icon="simple-icons:linkedin" color="black" height="28" /></a
      >
      <a href="https://codepen.io/bgass10" target="_blank">
        <Icon icon="simple-icons:codepen" color="black" height="28" />
      </a>
      <a href="https://replit.com/@BrendanGass" target="_blank">
        <Icon icon="simple-icons:replit" color="black" height="28" />
      </a>
      <a href="https://www.instagram.com/brendangass/" target="_blank">
        <Icon icon="simple-icons:instagram" color="black" height="28" />
      </a>
      <a href="https://twitter.com/BrendanGass" target="_blank">
        <Icon icon="simple-icons:twitter" color="black" height="28" />
      </a>
    </div>
  </div>
</div>

<style>
  .bg {
    position: absolute;
    top: 0;
    background-color: #f77909;
    width: 100vw;
    height: 100vh;
  }
  .wrapper {
    position: absolute;
    top: 0;
    width: 28px;
    height: 28px;
    margin-top: 3.7vh;
    margin-left: 84.5vw;
  }
  .nav {
    margin-left: 10vw;
    margin-right: 10vw;
    margin-top: 34vh;
  }
  h1 {
    color: black;
    font-family: Montserrat;
    font-size: 10vw;
    margin-top: 0;
    margin-bottom: 0.9vh;
  }
  .iconRow {
    display: flex;
    justify-content: space-between;
    margin-top: 1.8vh;
  }
  a:link,
  a:visited {
    text-decoration: none;
    cursor: pointer;
  }
</style>

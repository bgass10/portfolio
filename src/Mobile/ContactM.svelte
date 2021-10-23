<script>
  import Icon from "@iconify/svelte";
</script>

<section id="contact" class="main">
  <h1>Contact Me</h1>
  <h2>brendangass10@gmail.com</h2>
  <div class="iconRow">
    <a href="https://github.com/bgass10" target="_blank"
      ><Icon icon="simple-icons:github" color="#f77909" height="32" /></a
    >
    <a href="https://www.linkedin.com/in/brendangass/" target="_blank">
      <Icon icon="simple-icons:linkedin" color="#f77909" height="32" /></a
    >
    <a href="https://codepen.io/bgass10" target="_blank">
      <Icon icon="simple-icons:codepen" color="#f77909" height="32" />
    </a>
    <a href="https://replit.com/@BrendanGass" target="_blank">
      <Icon icon="simple-icons:replit" color="#f77909" height="32" />
    </a>
    <a href="https://www.instagram.com/brendangass/" target="_blank">
      <Icon icon="simple-icons:instagram" color="#f77909" height="32" />
    </a>
    <a href="https://twitter.com/BrendanGass" target="_blank">
      <Icon icon="simple-icons:twitter" color="#f77909" height="32" />
    </a>
  </div>
</section>

<style>
  .main {
    margin-left: 8vw;
    margin-right: 8vw;
  }
  h1 {
    color: white;
    font-family: Montserrat;
    font-size: 6.4vw;
    margin-top: 5.5vh;
    margin-bottom: 0;
  }
  h2 {
    color: white;
    opacity: 80%;
    font-family: Montserrat;
    font-size: 4.4vw;
    margin-top: 0.5vh;
  }
  .iconRow {
    display: flex;
    justify-content: space-between;
    margin-top: 1.8vh;
    margin-bottom: 3.6vh;
  }
</style>

<script>
  import Icon from "@iconify/svelte";
</script>

<section id="contact">
  <h1>Contact Me</h1>
  <h2>brendangass10@gmail.com</h2>
  <div class="row">
    <a href="https://twitter.com/BrendanGass" target="_blank">
      <Icon class="icon" icon="ci:twitter" height="36" />
    </a>
    <a href="https://www.instagram.com/brendangass/" target="_blank">
      <Icon class="icon" icon="ci:instagram" height="36" />
    </a>
  </div>
</section>

<style>
  section {
    margin-left: 15vw;
    margin-right: 15vw;
  }
  h1 {
    color: white;
    font-family: Montserrat;
    font-size: 2.3vw;
    margin-bottom: 0;
  }
  h2 {
    color: white;
    font-family: Montserrat;
    font-size: 1.1vw;
    margin-top: 0.6vh;
  }
  .row {
    display: flex;
  }
  div :global(.icon) {
    color: white;
    margin-right: 0.6vw;
    margin-bottom: 1.2vh;
  }
  div :global(.icon):hover {
    color: #f77909;
  }
</style>

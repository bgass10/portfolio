<script>
  export let projects;
  import Icon from "@iconify/svelte";
</script>

<section id="projects" class="main">
  <h1>Projects</h1>
  {#each projects as project}
    <div class="project">
      <h2>{project.title}</h2>
      <p>{project.desc}</p>
      <div class="iconRow">
        {#if project.gitSrc != false}
          <a href={project.gitSrc} alt="Link to project code." target="_blank">
            <Icon
              class="icon"
              icon="eva:github-outline"
              color="white"
              height="26"
            />
          </a>
        {/if}
        <a href={project.src} alt="Link to project." target="_blank">
          <Icon icon="fluent:open-20-filled" color="white" height="28" />
        </a>
      </div>
    </div>
  {/each}
</section>

<style>
  .main {
    margin-left: 8vw;
    margin-right: 8vw;
    padding-top: 3.7vh;
    margin-top: 4.6vh;
  }
  h1 {
    color: white;
    font-family: Montserrat;
    font-size: 7.5vw;
    margin-bottom: 0;
    margin-top: 0;
    text-align: center;
  }
  h2 {
    color: white;
    font-family: Montserrat;
    font-size: 6.4vw;
  }
  p {
    color: white;
    font-family: Montserrat;
    font-size: 4.2vw;
  }
  .project {
    margin-top: 2.4vh;
    background-color: #131313;
    padding-top: 1.4vh;
    padding-bottom: 3.2vh;
    padding-left: 7vw;
    padding-right: 3vw;
    border-radius: 4%;
  }
  div :global(.icon) {
    margin-right: 1.3vw;
  }
</style>

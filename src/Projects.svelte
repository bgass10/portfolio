<script>
  import Icon from "@iconify/svelte";

  export let projects;
</script>

<section id="projects" class="main">
  <h1>Projects</h1>
  <div class="row">
    {#each projects as project}
      <div class="project">
        <h2>{project.title}</h2>
        <p>{project.desc}</p>
        <div class="iconRow">
          {#if project.gitSrc != false}
            <a
              href={project.gitSrc}
              alt="Link to project code."
              target="_blank"
            >
              <Icon
                class="icon"
                icon="eva:github-outline"
                color="white"
                height="26"
              />
            </a>
          {/if}
          {#if project.src != false}
            <a href={project.src} alt="Link to project." target="_blank">
              <Icon icon="fluent:open-20-filled" color="white" height="28" />
            </a>
          {/if}
        </div>
      </div>
    {/each}
  </div>
</section>

<style>
  .main {
    margin-top: 10vh;
    margin-left: 15vw;
    margin-right: 15vw;
  }
  h1 {
    color: white;
    font-family: Montserrat;
    font-size: 4.15vw;
    margin-top: 1.2vh;
    margin-bottom: 2.4vh;
  }
  h2 {
    color: white;
    font-family: Montserrat;
    font-size: 1.6vw;
    margin-bottom: 0;
  }
  p {
    color: white;
    font-family: Montserrat;
    font-size: 0.93vw;
  }
  .row {
    display: flex;
    margin-top: 1.2vh;
    flex-wrap: wrap;
  }
  .iconRow {
    justify-self: baseline;
  }
  .project {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 20vw;

    margin-bottom: 2.25vw;
    padding-bottom: 1vw;
    padding-left: 1.5vw;
    margin-right: auto;
    background-color: #131313;
    border-radius: 4%;
  }
  .iconRow {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  div :global(.icon) {
    margin-right: 1.3vw;
  }
</style>

<script>
  import Icon from "@iconify/svelte";

  export let projects;
</script>

<section id="projects" class="main">
  <h1>Projects</h1>
  <div class="row">
    {#each projects as project}
      <div class="container">
        <img src={project.img} alt={project.desc} class="project" />
        <div class="overlayThru" />
        <div class="overlay">
          <div class="col">
            <div class="title">{project.title}</div>

            <div class="description">{project.desc}</div>
          </div>
          <div class="iconRow">
            {#if project.gitSrc != false}
              <a
                href={project.gitSrc}
                alt="Link to project code."
                target="_blank"
              >
                <Icon
                  class="icon"
                  icon="bx:bx-code-alt"
                  height="32"
                  hFlip={true}
                  style="margin: 10px"
                /></a
              >
            {/if}

            <a href={project.src} alt="Link to project." target="_blank">
              <Icon
                class="icon"
                icon="bx:bx-expand-alt"
                height="26"
                hFlip={false}
                style="margin: 10px"
              />
            </a>
          </div>
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
  .row {
    display: flex;
    margin-top: 1.2vh;
    flex-wrap: wrap;
  }
  .col {
    display: flex;
    flex-direction: column;
  }
  .title {
    color: white;
    text-align: center;
    font-size: 1.6vw;
    opacity: 1;
    font-family: Montserrat;
    margin-top: 2.4vh;
  }
  .description {
    color: white;
    text-align: center;
    font-size: 0.93vw;
    opacity: 1;
    font-family: Montserrat;
    margin-left: 0.6vw;
    margin-right: 0.6vw;
    margin-top: 0.6vh;
  }

  .container {
    width: 21.5vw;
    height: 26vh;
    margin-bottom: 2.25vw;
    margin-right: auto;
  }

  .project {
    width: 100%;
    height: 100%;
    border-radius: 7%;
  }

  .overlayThru {
    transform: translateY(-26.5vh);
    height: 100%;
    width: 100%;
    opacity: 0;
    transition: 0.3s ease;
    border-radius: 7%;
    background-color: #f77909;
  }
  .overlay {
    transform: translateY(-53vh);
    height: 100%;
    width: 100%;
    opacity: 0;
    transition: 0.5s ease;
    border-radius: 7%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  .container:hover .overlayThru {
    opacity: 0.8;
  }
  .container:hover .overlay {
    opacity: 1;
  }
  .iconRow {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  div :global(.icon) {
    color: rgb(243, 243, 243);
  }
  div :global(.icon):hover {
    color: white;
  }
</style>

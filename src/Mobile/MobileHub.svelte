<script>
  import IntroM from "./IntroM.svelte";
  import AboutM from "./AboutM.svelte";
  import ProjectsM from "./ProjectsM.svelte";
  import ContactM from "./ContactM.svelte";
  import Navigator from "./Navigator.svelte";

  export let projects;
  let inNavMode = false;
</script>

{#if !inNavMode}
  <IntroM bind:inNavMode />
  <AboutM />
  <ProjectsM {projects} />
  <ContactM />
{:else}
  <Navigator bind:inNavMode />
{/if}

<script>
  import LinkTray from "./LinkTray.svelte";
  import Navbar from "./Navbar.svelte";
  import Intro from "./Intro.svelte";
  import About from "./About.svelte";
  import Projects from "./Projects.svelte";
  import Contact from "./Contact.svelte";
  import MobileHub from "./Mobile/MobileHub.svelte";
  import { projects } from "./ProjectsData";

  let width;
  let height;
</script>

<svelte:window bind:outerWidth={width} bind:outerHeight={height} />

<svelte:head>
  <link
    href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&display=swap"
    rel="stylesheet"
  />
</svelte:head>

{#if width > 769 && width > height}
  <LinkTray />
  <Navbar />
  <Intro />
  <About />
  <Projects {projects} />
  <Contact />
{:else}
  <MobileHub {projects} />
{/if}

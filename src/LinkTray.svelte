<script>
  import Icon from "@iconify/svelte";
</script>

<div>
  <ul>
    <li>
      <a href="https://github.com/bgass10" target="_blank">
        <Icon class="white" icon="iconoir:github" height="28" />
      </a>
    </li>
    <li>
      <a href="https://www.linkedin.com/in/brendangass/" target="_blank">
        <Icon class="white" icon="feather:linkedin" height="28" />
      </a>
    </li>
    <li>
      <a href="https://codepen.io/bgass10" target="_blank">
        <Icon class="white" icon="iconoir:codepen" height="30" hFlip={true} />
      </a>
    </li>
    <li>
      <a href="https://replit.com/@BrendanGass" target="_blank">
        <Icon
          icon="simple-icons:replit"
          class="white"
          height="26"
          hFlip={true}
        />
      </a>
    </li>
    <li>
      <div class="line" />
    </li>
  </ul>
</div>

<style>
  .line {
    width: 0.11vw;
    background-color: #f77909;
    height: 15vh;
  }
  ul {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 0;
    position: fixed;
    left: 2.5vw;
    bottom: 0;
    margin-bottom: 0;
    list-style: none;
  }
  li {
    margin-top: 1.3vh;
  }
  div :global(.white) {
    color: white;
  }
  div :global(.white):hover {
    color: #f77909;
    transform: translateY(-0.6vh);
  }
</style>

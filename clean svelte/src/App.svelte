<script lang="ts">
  import svelteLogo from "./assets/svelte.svg";
  import viteLogo from "/vite.svg";
  import Counter from "./lib/Counter.svelte";
  let vite: string = "vite";
  let svelte: string = "svelte";
  let p2: string = " Click on the Vite and Svelte logos to learn more";
  let p1: string = "Check out ";
  let p1_1: string = "SvelteKit";
  let p1_2: string = "the official Svelte app framework powered by Vite!";
</script>

<main>
  <div>
    <a href="https://vitejs.dev" target="_blank" rel="noreferrer">
      <img src={viteLogo} class="logo" alt="Vite Logo" />
    </a>
    <a href="https://svelte.dev" target="_blank" rel="noreferrer">
      <img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
    </a>
  </div>
  <h1>{vite} + {svelte}</h1>

  <div class="card">
    <Counter />
  </div>

  <p>
    {p1} <a
      href="https://github.com/sveltejs/kit#readme"
      target="_blank"
      rel="noreferrer">{p1_1}</a
    >,{p1_2}
  </p>
  {p2}
  <p class="read-the-docs" />
</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }

  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }

  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }

  .read-the-docs {
    color: #888;
  }
</style>

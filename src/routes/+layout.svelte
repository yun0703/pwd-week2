<script>
  import { resolve } from '$app/paths';

  let { children } = $props();
</script>

<svelte:head>
  <title>AJOU Mini Portfolio</title>
  <meta name="description" content="SvelteKit + Vercel mini portfolio" />
</svelte:head>

<nav>
  <a href={resolve('/')}>Home</a>
  <a href={resolve('/about')}>About</a>
  <a href={resolve('/projects')}>Projects</a>
</nav>

<main>
  {@render children()}
</main>

<style global>
  @import '../app.css';
</style>
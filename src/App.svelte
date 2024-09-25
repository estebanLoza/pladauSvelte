<script>
  // import svelteLogo from './assets/svelte.svg';
  // import viteLogo from '/vite.svg';
  import Footer from "./Components/footer.svelte";
  import Navbar from "./Components/Navbar.svelte";
  import InicioDos from "./lib/InicioDos.svelte";

  import "../src/app.css";
</script>

<div class="layout">
  <Navbar />
  <main>
    <slot />
  </main>
  <Footer />
</div>

<style>
  .layout{
    display: grid;
    grid-template-columns: 1fr auto;
    }
</style>

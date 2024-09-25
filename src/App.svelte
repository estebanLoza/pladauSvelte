<script>
  import Navbar from "./Components/Navbar.svelte";

</script>


<div class="layout">
  <Navbar />

  <main>
    <slot />
  </main>

  <footer>
    <p>este es un componente footer</p>
  </footer>
</div>


<style>

  main{
    display: flex;
    flex-direction: column;  
    min-height: 100vh;
  }
  footer{
    background-color: green;

  }


</style>

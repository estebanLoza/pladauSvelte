<script>
    //Importacion del logo de la empresa
    import PLADAU from '../img/PLADAU.png';
  
      //variable para la navegacion y import de los componentes
    export let menu = 1;
    import Inicio from "../lib/Inicio.svelte";
    import Nosotros from "../lib/Nosotros.svelte";
</script>

<header>
  <nav>
    <div>
      <img src={PLADAU} alt="Logo de la empresa PLADAU">
    </div>
    <ul id="menu">
      <li><a href="/" on:click|preventDefault={() => (menu = 1)}>Inicio</a></li>
      <li><a href="/" on:click|preventDefault={() => (menu = 2)} >Nosotros</a></li>
      <li><a href="/" on:click|preventDefault={() => (menu = 3)} >Facultades</a></li>
      <li><a href="/" on:click|preventDefault={() => (menu = 4)} >Inicio Sesión</a></li>
      <li><a href="/" on:click|preventDefault={() => (menu = 5)} >Resgistrarse</a></li>
    </ul>
  </nav>
</header>
{#if menu === 1}
  <Inicio />
{:else if menu === 2}
  <Nosotros />
{/if}


<style>
  header{
    width: 100%;
    height: 5.625rem;
    background-color:#6E98D8;
  }
  
  nav{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  /*CAJA DEL LOGO*/
  nav div{
    border:1px solid red;
    margin-left: 2%;
  }
  
  
  nav ul {
    border: 0.5px solid green;
    display: flex;
    justify-content: flex-end;
    gap:5%;
    margin-right: 3%;
  }
  
  nav ul li{
    list-style: none;
  }
  
  nav ul a{
    font-family: kodchasan;
    text-decoration:none;
    color: white;
    padding: 15%;
  }
  nav ul a:hover{
    background-color: green;
    border-radius: 15%;
  }
</style>
<script>
    //Importacion del logo de la empresa
    import PLADAU from '../img/PLADAU.png';
  
      //variable para la navegacion y import de los componentes
    export let menu = 1;
    import Inicio from "../lib/Inicio.svelte";
    import Nosotros from "../lib/Nosotros.svelte";
    import Facultades from "../lib/Facultades.svelte";
    import InicioSesion from "../lib/InicioSesion.svelte";
    import Registrarse from '../lib/Registrarse.svelte';
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


<!--?Codigo para el NavBar-->
{#if menu === 1}
  <Inicio />
{:else if menu === 2}
  <Nosotros />
{:else if menu === 3}
  <Facultades />
{:else if menu === 4}
  <InicioSesion />
{:else if menu === 5}
  <Registrarse />
{/if}





<style>
  header{
    width: 100%;
    height: 6rem;
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
    margin-left: 2%;
  }
  
  
  #menu {
    width: 50%;
    display: flex;
    justify-content: flex-end;
    gap:1%;
    margin-right: 3%;
  }
  
  #menu li{
    list-style: none;
  }

  #menu li:nth-child(5){
    background-color: white; 
    border-radius: 0.3em;
    padding:0.2rem;
  }


  #menu li:nth-child(5) a{ /**nth-child, solo funciona con hijos directos de su padre (en este caso ul)*/
    color: black;
  }

  #menu li:nth-child(5) a:hover{
    background-color: black;
    color: white;
    width: 100%;
  }

  
  #menu li a{
    font-family: kodchasan;
    text-decoration:none;
    color: white;
    padding: 0.2rem;
    font-size: 120%;
    font-weight: 700;

  }

  #menu li:not(:nth-child(5)) a:hover {
    background-color: green;
    border-radius: 0.3em;
  }

</style>
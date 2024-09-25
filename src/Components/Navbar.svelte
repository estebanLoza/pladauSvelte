<script>
  //Importacion del logo de la empresa
  import PLADAU from "../../public/img/PLADAU.png";

  //Importacion de Router, Link, Route para la navegación
  import { Router, Link, Route } from "svelte-routing";

  
  import Nosotros from "../lib/Nosotros.svelte"; //Esto son las variables para la navegación
  import Facultades from "../lib/Facultades.svelte";
  import InicioSesion from "../lib/InicioSesion.svelte";
  import Registrarse from "../lib/Registrarse.svelte";
  import Inicio from "../lib/InicioDos.svelte";
  
</script>

<header>
  <Router>
    <nav>
      <div>
        <img src={PLADAU} alt="Logo de la empresa PLADAU" />
      </div>
      <div class="nav-link">
        <Link class="botoneslink" to="/Inicio">Inicio</Link>
        <Link class="botoneslink" to="/Nosotros">Nosotros</Link>
        <Link class="botoneslink" to="/Facultades">Facultades</Link>
        <Link class="botoneslink" to="/InicioSesion">Inicio Sesion</Link>
        <Link class="botoneslink" to="/Registrarse">Registarse</Link>
      </div>
    </nav>
    <!-- Código para la navegación de rutas en Svelte -->
    <Route path="/Inicio" component={Inicio} />
    <Route path="/Nosotros" component={Nosotros} />
    <Route path="/Facultades" component={Facultades} />
    <Route path="InicioSesion" component={InicioSesion} />
    <Route path="/Registrarse" component={Registrarse} />
  </Router>
</header>

<style>
  header {
    width: 100%;
    height: 5em;
    background-color: #6e98d8;
  }

  nav {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0em 2em 0em 2em;
    font-family: kodchasan;
  }


.nav-link{
    display:inline-flex;
    color: white;
    gap:1.5em;
  }  


  :global(.botoneslink){  /*Al componentes de svelte se tiene que agregar con global, paar que funcione (lo estoy haciendo esta página con svelte+vite) */
    color: white;
    font-family: kodchasan;
    font-weight: 700;
    font-size: 1.2em;
    text-decoration: none;
    padding: 0.3em;
  }


  :global(.botoneslink:hover:not(:nth-child(5))){ /*Esto indica que el ultimo componente no usará el background-color en verde**/
    background-color:rgb(50, 211, 50);
    border-radius: 8%;
  }

  

  :global(.botoneslink:nth-child(5)){
    background-color: white;
    color: black;
    border-radius: 8%;
  } 

  :global(.botoneslink:nth-child(5):hover){
    background-color: rgb(131, 231, 100);
    color: rgb(255, 253, 253);
  }










</style>

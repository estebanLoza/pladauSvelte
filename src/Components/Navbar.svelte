<script>
  //Importacion del logo de la empresa
  import PLADAU from "../img/PLADAU.png";

  //Importacion de Router, Link, Route para la navegación

  import { Router, Link, Route } from "svelte-routing";

  import Inicio from "../lib/Inicio.svelte";
  import Nosotros from "../lib/Nosotros.svelte"; //Esto son las variables para la navegación
  import Facultades from "../lib/Facultades.svelte";
  import InicioSesion from "../lib/InicioSesion.svelte";
</script>

<header>
  <Router>
    <nav>
      <div>
        <img src={PLADAU} alt="Logo de la empresa PLADAU" />
      </div>
      <Link
        class="botones-link"
        style="color:white;
        color: #fff; /* Cambia el color del texto */
        text-decoration: none; /* Quita el subrayado */
        padding: 10px; /* Espacio alrededor del texto */
        transition: color 0.3s; /* Efecto de transición al cambiar de color */
      "
        to="/Inicio">Inicio</Link
      >
      <Link class="botones-link" 
        style="color:white;
        color: #fff; /* Cambia el color del texto */
        text-decoration: none; /* Quita el subrayado */
        padding: 10px; /* Espacio alrededor del texto */
        transition: color 0.3s; /* Efecto de transición al cambiar de color */"

        to="/Nosotros">Nosotros</Link>
      <Link class="botones-link" 
        style="color:white;
        color: #fff; /* Cambia el color del texto */
        text-decoration: none; /* Quita el subrayado */
        padding: 10px; /* Espacio alrededor del texto */
        transition: color 0.3s; /* Efecto de transición al cambiar de color */"

      
        to="/Facultades">Facultades</Link>
      <Link class="botones-link" 
        style="color:white;
        color: #fff; /* Cambia el color del texto */
        text-decoration: none; /* Quita el subrayado */
        padding: 10px; /* Espacio alrededor del texto */
        transition: color 0.3s; /* Efecto de transición al cambiar de color */
        "
      
        to="/InicioSesion">Inicio Sesion</Link>
    </nav>
    <!-- Código para la navegación de rutas en Svelte -->
    <Route path="/Inicio" component={Inicio} />
    <Route path="/Nosotros" component={Nosotros} />
    <Route path="/Facultades" component={Facultades} />
    <Route path="InicioSesion" component={InicioSesion} />
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

  /* nav .botones-link {
        color: #fff; /* Cambia el color del texto */
  /* text-decoration: none; /* Quita el subrayado */
  /* padding: 10px; /* Espacio alrededor del texto */
  /* transition: color 0.3s; Efecto de transición al cambiar de color */
  /* } */

  /* nav .botones-link:hover {
        color: #ffcc00; Cambia el color al pasar el mouse */
  /* } */
</style>

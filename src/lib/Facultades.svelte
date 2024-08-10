<script>
  //Importaciones de Imagenes Iconos de Facultades
  
  import Fime from "../img/ImgPladau/Ellipse FIME.png";
  import Facpya from "../img/ImgPladau/Ellipse FACPYA.png";
  import Facdyc from "../img/ImgPladau/Ellipse FACDYC.png";
  import Farq from "../img/ImgPladau/Ellipse FARQ.png";
</script>

<main>
  <section id="sec1">
    <div id="titulo"><h1>FACULTADES</h1></div>
    
    <div id="parrafoFacultades">
      <p>
        Aquí encontraras las facultades de la Universidad Atunoma de Nuevo León (UANL), donde veras la facultad donde estudias, o si en el caso que aun no estudias la facultad, aqui podras ver lo que aprende un estudiante de esa universidad y lo que puedes aprender desde antes que empiezas a estudiarlo.
      </p>
    </div>
  </section>
  
  <!--*Diseño de las facutlades-->
  
  <section id="sec2">
    <div id="grid-Facultades">
        <div class="facu-Seleccion">
          <img src={Fime} alt="Logo de la facultade Fime UANL">
        </div>
        <div class="facu-Seleccion">
          <img src={Farq} alt="Logo de la facultade Farq UANL">
        </div>
        <div class="facu-Seleccion">
          <img src={Facdyc} alt="Logo de la facultad Facdyc UANL">
        </div>
        <div class="facu-Seleccion">
          <img src={Facpya} alt="Logo de la facultad de Facpya UANL">
        </div>
    </div>
  </section>
</main>



<style>
  #sec1{
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top:2%;
  }
  
  #titulo h1{
    font-family:kodchasan;
  }
  
  #parrafoFacultades {
    width: 50%;
  }
  
  #parrafoFacultades p{
    font-family: kodchasan;
    font-size: 1rem;
    font-weight: bold;
  }
  
  
  /**Diseño de las facultades con Grid*/
  #sec2{
    display: flex;
    justify-content: center;
    margin-top: 10%;
    width: 100%;
  }
  
  #grid-Facultades{
    display:grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-template-rows: 100%;
    gap: 15%;
  }
  
  
</style>
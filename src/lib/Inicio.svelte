<script>
  //importacion de imagenes
  
  import Bienvenida from "../img/Rectangle 3.png";
  import GrupoEstudiantes from "../img/Rectangle 6.png";
</script>


<div class="Bienvenida"
      style="background-image:url({Bienvenida});
              width: 100%;
              height: 80vh;
              background-position: center center;
              background-repeat: no-repeat;
              background-size: cover;
            
    ">
  
      <!--Contenedor de bienvenida-->
      <div class="BienvenidoAutodidacta" style="
                  background-color:rgba(11, 11, 11, 0.65);
                  width: 60vw;
                  height: 20vh;
                  border-radius: 1rem;
                  display: flex;
                  flex-direction: column;
                  justify-content: center;
                  align-items: center;
                  position: relative;
                  left: 20%;
                  top: 25%;
                  ">
        <h1>BIENVENIDO AUTODIDACTA</h1>
        <h6>TE AYUDAREMOS A FORMARTE EN LO PROFESIONAL</h6>
      </div>

</div>


<main>
  <section>
    <div id="textoInfo">
      <p>
        Te ayudaremos con el material necesario para que pases la materia, desde la facultad que estudias hasta los libros
        y videos que usan los estudiantes de esa facultad.
        Pero, si eres un estudiante de preparatoria, tambien veras lo que estudia un ingeniero electronico, abogado, etc.
        Y así, sabras si realmente es lo que quieres.
      </p>
    </div>

    <figure>
      <img src={GrupoEstudiantes} alt="Grupo de estudiantes Imagen ilustrativa">
    </figure>
    
  </section>
</main>




<style>
.BienvenidoAutodidacta h1, .BienvenidoAutodidacta h6{
  color: white;
  font-family: kodchasan;
  
}

main{
  height:50vh;
  width: 100%;
}
section{
  height: 100%;
  width: 100%;
  display: flex;
}

#textoInfo{
  background-color:#556E85;
}

#textoInfo p{
  font-size: 1.4rem;
  font-family: kodchasan;
  color: white;
  padding: 2.32rem;
}

figure{
  height: 100%;
  width: 50%;
}
figure img{
  height: 100%;
  object-fit: cover;
  
  
}
</style>
<script>
  //Img
  import Welcome from "../../public/img/Rectangle 3.png";
  import Estudiante1 from "../../public/img/Rectangle 6.png";
  import App from "../App.svelte";
</script>

<main>
  <div class="backgroundImg" style="background-image:url({Welcome});">
    <div class="welcomeAuto">
      <p>Bienvenido autodidacta</p>
      <p>Te ayudaremos con tu progreso</p>
    </div>
  </div>

  <div class="section1" style="display:flex; width:100%;">
    <div class="sectionText1" style="width:50%;">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium
      laborum doloribus cumque ducimus dolorem alias necessitatibus similique
    </div>
    <div class="sectionImg1" style="width: 50%;">
      <img src={Estudiante1} alt="Grupo de estudiantes" />
    </div>
  </div>
</main>

<style>
  main {
    margin: 0;
    padding: 0;
  }

  .backgroundImg {
    width: 100%;
    height: 65vh;
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
  }

  .welcomeAuto {
    background-color: rgba(27, 26, 26, 0.884);
    width: 35%;
    height: 45%;
    position: relative;
    left: 35%;
    top: 25%;
    border-radius: 11%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .welcomeAuto p {
    color: white;
    font-family: kodchasan;
    font-weight: bold;
  }

  .welcomeAuto p:nth-child(1) {
    font-size: 2em;
  }

  .welcomeAuto p:nth-child(2) {
    font-size: 1.2em;
  }

  .section1{
    width: 100%;
    height: 43vh;
  }
/**Diseño section*/
  .sectionText1{
    background-color: #264B6C;
    width: 50%;
    height: 100%;
  }

  .sectionImg1{
    width: 50%;
    height: 100%;
  }

  .sectionImg1 img{
    width: 100%;
    height: 100%;
    object-fit: cover;

  }


</style>

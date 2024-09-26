<script>
  import WelcomeImg from "../../public/img/Rectangle 3.png";

  import Friends from "../../public/img/Rectangle 6.png";

  import logo from "../../public/img/PLADAU.png";


  import Footer from "../Components/Footer.svelte";
</script>

<div class="layoutInicio">
  <div class="BoxBackground" style="background-image: url({WelcomeImg});">
    <div></div>
  </div>

  <div class="Section1">
    <div class="secTex1">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi dolore
        animi laboriosam harum, sunt quibusdam colum
      </p>
    </div>
    <div class="BoxImg1">
      <img src={Friends} alt="Grupo de estudiantes" />
    </div>
  </div>

  <div class="Section1">
    <div class="secTex1">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi dolore
        animi laboriosam harum, sunt quibusdam colum
      </p>
    </div>
    <div class="BoxImg1">
      <img src={Friends} alt="Grupo de estudiantes" />
    </div>
  </div>

  <div class="Section1">
    <div class="secTex1">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi dolore
        animi laboriosam harum, sunt quibusdam colum
      </p>
    </div>
    <div class="BoxImg1">
      <img src={Friends} alt="Grupo de estudiantes" />
    </div>
  </div>

  <div class="Section1">
    <div class="secTex1">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi dolore
        animi laboriosam harum, sunt quibusdam colum
      </p>
    </div>
    <div class="BoxImg1">
      <img src={Friends} alt="Grupo de estudiantes" />
    </div>
  </div>
</div>


<Footer/>





<style>
  .BoxBackground {
    width: 100%;
    height: 64vh;
    background-position: center center;
    background-repeat: no-repeat;
    background-size: cover;
  }


  .Section1{
    border: 1px solid red;
  }
</style>

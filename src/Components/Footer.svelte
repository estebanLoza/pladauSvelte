
  
  <script>
    import logo from "../../public/img/PLADAU.png";
  </script>
  
  
  <!--Footer para inicio-->
  <footer>
    <figure>
      <img src={logo} alt="Logo de la empresa PLADAU" />
    </figure>
    <div>
      <ul>
        <li>Punto</li>
        <li>Punto2</li>
        <li>Punto3</li>
      </ul>
    </div>
</footer>


<style>

  footer{
    background-color: #6e98d8;
    height: 6.5em;
    display: flex;
    align-items: center;
    justify-content: space-around;
    }
  /**Esto estilos de main y footer, hace que el footer quede abajo siempre con el minimo de 100vh de la ventana*/

   footer figure{
    height: 100%;
    border: 1px solid green;
    display: flex;
    align-items: center;

  } 

</style>
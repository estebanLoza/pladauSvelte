<script></script>

<main>
  <h1>Regístrate y comienza a aprender.</h1>

  <form action="">
    <!--*Secciones de Input de Nombre, correo, contraseña-->
    <div>
      <input type="text" placeholder="Nombre Completo" id="text" required />
    </div>

    <div>
      <input
        type="email"
        placeholder="Correo electrónico"
        id="email"
        required
      />
    </div>

    <div>
      <input type="password" placeholder="Contraseña" id="password" required />
    </div>

    <!--*Seccion de checkbox sobre los terminos-->

    <div class="cajaCheckbox">
      <label class="checkbox-terms">
        <input type="checkbox" required />
        <p>Acepto términos y condiciones</p>
      </label>
    </div>
    <div class="cajaCheckbox caja2Checkbox">
      <label class="checkbox-terms">
        <input type="checkbox" />
        <p>
          Quiero recibir ofertas especiales, recomendaciones personalidades y
          consejos de aprendizaje
        </p>
      </label>
    </div>

    <!--*Caja de Submit-->
    <div>
      <input type="submit" value="Regístrate" />
    </div>
  </form>
</main>

<style>
  main {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  h1 {
    font-family: kodchasan;
    margin-top: 2rem;
    margin-bottom: 2rem;
  }
  input[type="text"]::placeholder,
  input[type="email"]::placeholder,
  input[type="password"]::placeholder {
    font-family: kodchasan;
    color: black;
    font-size: 1rem;
    padding: 1rem;
  }

  #text,
  #email,
  #password {
    width: 35.34rem;
    height: 6rem;
    border-radius: 0.94rem;
    background-color: #f5f3f3;
    border: 2px solid black;
    margin-top: 5%;
  }

  input[type="submit"] {
    margin-top: 1em;
    padding: 0.5rem;
    background-color: #007bff;
    color: white;
    border: none;
    cursor: pointer;
    font-family: kodchasan;
  }

  /* Estilo para el placeholder, excluyendo los input de tipo submit */
  input[type="checkbox"] {
    width: 1rem;
    height: 2rem;
  }

  .cajaCheckbox {
    display: flex;
    align-items: center;
    /*  border:1px solid black;*/
    margin-top: 1%;
  }

  .checkbox-terms{
    display: flex;
    align-items: center;
    
  }
</style>

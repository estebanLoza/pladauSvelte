<script>

    import IconoInicio from "../img/Ellipse 19.jpg";


    //Icono de Google, Facebook, Apple
    import IconoGoogle from "../img/googleicon 1.png";
    import IconoFacebook from "../img/facebookicon 1.png";
    import IconoApple from "../img/appleicon(company) 1.png";


</script>



<main> 
    <div class="TituloYImagen">
        <h1>INICIO DE SESIÓN</h1>

    </div>

    <figure>
        <img src={IconoInicio} alt="ICONO DE FOTO DE INICIO">
    </figure>

    <form>
        <div class="contenedorInfo">
            <label for="text">Username</label>
            <input type="text" id="usuario">
        </div>

        <div class="contenedorInfo caja2" >
            <label for="password">Password</label>
            <input type="password" id="password">
        </div>
        
        <div class="contenedorInfo cajaBoton" >
            <label for="submit">
                <input type="submit" value="INICIAR SESIÓN">
            </label>
        </div>
    </form>

    <div class="Iconos-caja">
        <img src={IconoGoogle} alt="Icono de Google">
        <img src={IconoFacebook} alt="Icono de Facebook">
        <img src={IconoApple} alt="Icono de Apple">
    </div>

    <div id="OpcionInicioSesion">
        <a href=".">Inicia sesión con tu organización</a>
    </div>

      
        
      


</main>





<style>
    main{
        width: 100%;
        height: auto;
        display: flex;
        flex-direction: column;
        align-items: center;

    }
    form{
        margin: 3% 0% 3% 0%;
    }

    .TituloYImagen{
        margin-top: 3%;
    }

    .TituloYImagen h1{
        font-family: kodchasan;
    }


    .contenedorInfo label{
        display: block;
        margin-bottom: 2%;
        font-family: kodchasan;
    }

    input[type=text], input[type=password]{
        border: none;
        border-bottom: 1px solid black;
        padding: 0.5rem 0;
        box-sizing: border-box;
        width: 100%;
    }

    .caja2{ /**Este class esta dentro del form, es el div 2*/
        margin-top: 10%;
    }


    input[type=submit]{
        width: 20vw;
        height: 10vh;
        background-color:#69DC41;
        border:none;
        color: white;
        border-radius: 1em;
        font-size: 1.4rem;
        font-weight: bold;
    }

    input[type=submit]:hover{
        background-color: white;
        color: black;
        border: 1px solid black;
    }

    .cajaBoton{
        display: flex;
        justify-content: center;
        margin-top: 10%;
    }

    label[for=text], label[for=password]{
        font-size: 1.5rem;
        font-weight: 500;
    }

    .Iconos-caja{
        display: flex;
        gap: 2em;
    }


    #OpcionInicioSesion{
        margin-top: 2rem;
    }

    #OpcionInicioSesion a{
        color:#29A000;
        font-size: 1.4rem;
        font-family: bold;
        font-family: kodchasan;
    }


</style>
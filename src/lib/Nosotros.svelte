<script>
    import Footer from "../Components/Footer.svelte";
    import Fachada from "../../public/img/fime-fachada.png";
</script>

<div class="layoutNosotros" style="
    width: 100%;
    min-height: 100vh;
    background-image:url({Fachada});
">
    <div class="BoxNosotros">
        <div class="BoxInfo">
            <div>

            </div>
        </div>
    </div>
</div>



<Footer/>



<style>
    .layoutNosotros{
        background-position: center center;
        background-repeat: no-repeat;
        background-size: cover;
    }

    .BoxNosotros{
        position: relative;
        left: 15%;
        width: 65%;
        height: 55vh;
        background-color: rgba(0, 0, 0, 0.603);
    }
</style>

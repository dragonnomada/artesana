<template>
    <ArtesanaHeaderLight page="historias" />
    <div class="artesana-welcome">
        <div class="artesana-title">
            <h1>Aprende en familia y a tu ritmo</h1>
        </div>
        <div class="artesana-description">
            <span>Toma nuestros cursos para que mejores la comercialización de tus productos progresivamente. Los
                contenidos son sencillos, breves y específicos.</span>
        </div>
        <div class="artesana-register-container">
            <div class="artesana-register-button">
                <span>Ir a Cursos</span>
            </div>
        </div>
        <div>
            <div class="artesana-esfera"></div>
        </div>
        <ArtesanaGaleria />
        <EtsyLogo />
    </div>
</template>

<script setup>
import ArtesanaHeaderLight from './ArtesanaHeaderLight.vue';
import EtsyLogo from './EtsyLogo.vue';
import ArtesanaGaleria from './ArtesanaGaleria.vue';
</script>

<style scoped>
.artesana-welcome {
    min-height: 50vh;

    position: relative;

    display: flex;
    flex-direction: column;

    padding: 64px 48px;

    zoom: 1.5;
}

.artesana-esfera {
    position: absolute;
    top: calc(40% - 100px);
    right: calc(20% - 100px);

    width: 180px;
    height: 180px;
    
    border-radius: 50%;

    background: linear-gradient(-30deg, rgb(0, 127, 244) 20%, rgb(244, 88, 0) 80%);
}

.artesana-register-container {
    display: flex;

    padding: 24px 0px;
}

.artesana-description {
    max-width: 500px;
}

.artesana-register-button {
    border: 1px solid black;
    padding: 6px 12px;
}
</style>
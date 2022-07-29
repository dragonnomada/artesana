<template>
    <div class="artesana-welcome">
        <div class="artesana-title">
            <h1>Bienvenido a la casa del artesano</h1>
        </div>
        <div class="artesana-description">
            <span>Esta es tu casa donde podrás abrir tu tienda y darle seguimiento a tus ventas, aprender a promover tus
                productos y convertirte en la nueva historia de éxito</span>
        </div>
        <div class="artesana-register-container">
            <div class="artesana-register-button">
                <span>Registrate</span>
            </div>
        </div>
        <EtsyLogo />
    </div>
</template>

<script setup>
import EtsyLogo from './EtsyLogo.vue';
</script>

<style scoped>
.artesana-welcome {
    min-height: 50vh;

    position: relative;

    display: flex;
    flex-direction: column;
    justify-content: center;

    padding: 64px 48px;

    zoom: 1.5;
}

.artesana-register-container {
    display: flex;

    padding: 24px 0px;
}

.artesana-description {
    max-width: 500px;
}

.artesana-register-button {
    background-color: #007FF4;
    border-radius: 20px;
    padding: 6px 12px;
}
</style>
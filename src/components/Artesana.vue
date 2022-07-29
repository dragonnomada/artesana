<template>
    <div class="artesana">
        <ArtesanaHeader />
        <ArtesanaWelcome />
        <ArtesanaPreview />
    </div>
</template>

<script setup>
import ArtesanaHeader from './ArtesanaHeader.vue';
import ArtesanaWelcome from './ArtesanaWelcome.vue';
import ArtesanaPreview from './ArtesanaPreview.vue';
</script>

<style scoped>
.artesana {
    width: 100%;
    height: 100vh;

    display: flex;
    flex-direction: column;

    background: linear-gradient(-125deg, rgb(0, 127, 244), rgb(244, 88, 0) 110%);
    color: white;
}
</style>
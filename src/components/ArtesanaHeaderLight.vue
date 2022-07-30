<template>
    <div class="artesana-header" :class="{ scroll: scroll >= 100 }">
        <div class="artesana-logo" @click="openPage('home')">
            <span>arte</span>
            <span>sana</span>
        </div>
        <div class="artesana-menu">
            <div class="artesana-sites">
                <div class="artesana-sites-item" :class="{ active: props.page === 'historias' }"
                    @click="openPage('historias')">
                    <span>Historias</span>
                </div>
                <div class="artesana-sites-item" :class="{ active: props.page === 'nosotros' }"
                    @click="openPage('nosotros')">
                    <span>Nosotros</span>
                </div>
                <div class="artesana-sites-item" :class="{ active: props.page === 'aprender' }"
                    @click="openPage('aprender')">
                    <span>Aprender</span>
                </div>
                <div class="artesana-sites-item" :class="{ active: props.page === 'miTienda' }"
                    @click="openPage('miTienda')">
                    <span>MiTienda</span>
                </div>
                <div class="artesana-sites-item" :class="{ active: props.page === 'ayuda' }"
                    @click="openPage('ayuda')">
                    <span>Ayuda</span>
                </div>
            </div>
            <div class="artesana-store-container">
                <div class="artesana-store-button">
                    <span>Abre tu tienda Etsy</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { inject } from 'vue';

const props = defineProps({
    page: {
        type: String,
        default: "none"
    }
})

const openPage = inject('page/@change')
</script>

<style scoped>
.artesana-header {
    width: 100%;

    position: fixed;
    left: 0px;
    top: 0px;

    display: flex;

    align-items: center;

    padding: 24px 48px;


    box-sizing: border-box;

    z-index: 100;
}

.scroll {
    background: linear-gradient(-125deg, rgb(0, 127, 244), rgb(244, 88, 0) 140%);
}

.artesana-logo {
    cursor: pointer;

    display: flex;

    font-size: 1.5rem;
}

.artesana-logo>span:nth-child(1) {
    font-weight: 600;
}

.artesana-logo>span:nth-child(2) {
    font-weight: 200;
}

.artesana-menu {
    flex-grow: 1;

    display: flex;
    justify-content: end;
    align-items: center;
}

.artesana-sites {
    display: flex;
}

.artesana-sites-item {
    padding: 0px 12px;

    cursor: pointer;
}

.artesana-sites-item:hover {
    text-decoration: underline;
}

.artesana-sites-item.active {
    text-decoration: underline;
    font-weight: 600;
}

.artesana-store-button {
    border: 1px solid black;
    border-radius: 20px;
    padding: 6px 12px;

    font-weight: 600;
}
</style>
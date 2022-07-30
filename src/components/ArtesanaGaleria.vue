<template>
<div class="galeria">
            <div class="flecha izq">
            <span><i class="fa-solid fa-chevron-left"></i></span>
            </div>
            <div class="galeria-scroll">
                <template v-for="item in galeria" key="item.id">
                    <div class="galeria-item">
                        <div class="galeria-item-picture">
                            <img :src="item.picture" alt="">
                        </div>
                        <div class="galeria-item-title">
                            <span>{{ item.title }}</span>
                        </div>
                        <div class="galeria-item-content">
                            <span>{{ item.content }}</span>
                        </div>
                    </div>
                </template>
            </div>
            <div class="flecha der">
            <span><i class="fa-solid fa-chevron-right"></i></span>
            </div>
        </div>
</template>

<script setup>
import { ref } from 'vue';

const galeria = ref([
    {
        id: 1,
        picture: "https://static.overlay-tech.com/assets/94bf379e-3ea0-444f-85d1-9ae1e139e5ca.png",
        title: "Diseño de marca",
        content: "La identidad de marca te ayudará a expresar mejor la calidad de tus artesanías"
    },
    {
        id: 2,
        picture: "https://static.overlay-tech.com/assets/9e5072b9-faea-407a-8d88-4ca847d2f865.png",
        title: "Introducción a la fotografía comercial",
        content: "Las imágenes de tus productos son clave para conectar con el cliente"
    },
    {
        id: 3,
        picture: "https://static.overlay-tech.com/assets/a5615a3b-ed0e-4897-87d7-8fb49c63a023.png",
        title: "Packeging",
        content: "Aprende la importancia de darle la terminación adecuada a tu producto"
    },
    {
        id: 4,
        picture: "https://static.overlay-tech.com/assets/9e2a99c6-e4e3-4c45-a53e-fb644c371620.png",
        title: "Organización de ferias",
        content: "El diseño de espacios para la venta de tus productos te ayuda a fortalecer tu negocio"
    },
])
</script>

<style scoped>

.galeria {
    width: 70%;

    display: flex;
    align-items: center;

    overflow: hidden;
}

.galeria-scroll {
    display: flex;
    align-items: flex-start;
    
    overflow-x: auto;
}

.flecha {
    padding: 0px 24px;
}

.galeria-item {
    display: flex;
    flex-direction: column;
    align-items: center;

    font-size: 0.6rem;

    padding: 24px;
}

.galeria-item-picture > img {
    width: 80px;
    height: 80px;
    object-fit: cover;
}

.galeria-item-title {
    padding: 12px 0px;
    font-weight: 600;

    text-align: center;
}
.galeria-item-content {
    text-align: center;
}
</style>
<template>
  <div class="artesana-preview">
    <p class="title">
      Así de sencillo es alcanzar el éxito
    </p>
    <p class="description">
      Promueve ventas las 24 horas del día, los 365 días del
      año, a millones de clientes
      <strong class="description-emphasis-1">Etsy</strong>
    </p>
    <div class="flex-wrapper-one">
      <div class="start-button">
        <p class="start-button-text">Comenzar a vender</p>
      </div>
      <div class="more-button">
        <p class="more-button-text">Historias de éxito</p>
      </div>
    </div>
    <div class="flex-wrapper-two">
      <div class="store-now">
        <img
          alt=""
          class="store-now-icon"
          src="https://static.overlay-tech.com/assets/dcc1a615-d78c-420e-b4a7-db26da990ea6.svg"
        />
        <p class="store-now-title">Abre tu Tienda Etsy</p>
        <p class="store-now-description">
          Inicia el camino para llegar a millones de
          clientes en más de 70 países.
        </p>
      </div>
      <div class="store-story">
        <img
          alt=""
          class="store-story-icon"
          src="https://static.overlay-tech.com/assets/730715d3-a40d-4e0c-94d8-15ca3a2410fc.svg"
        />
        <p class="store-story-title">
          Cuéntanos tu historia
        </p>
        <p class="store-now-description">
          Acércate al cliente a través de tu historia, la de
          tus artesanías y la de tu comunidad para más y
          mejores ventas.
        </p>
      </div>
      <div class="store-now">
        <img
          alt=""
          class="store-improve-icon"
          src="https://static.overlay-tech.com/assets/49ad1039-2010-4c11-a25a-acd6e11eddc5.svg"
        />
        <p class="store-improve-title">
          Mejorar tu negocio
        </p>
        <p class="store-now-description">
          Con nuestro programa de aprendizaje a tu manera,
          crecemos juntos en la realización de mejores
          formatos de venta.
        </p>
      </div>
    </div>
    <EtsyLogo />
  </div>
</template>

<script setup>
import EtsyLogo from './EtsyLogo.vue';
</script>

<style lang="scss" scoped>
.artesana-preview {
  position: relative;

  display: flex;
  flex-direction: column;
  align-items: flex-start;

  padding: 128px 64px;
}
.title {
  height: 10.49%;
  width: 83.2%;
  font-family: "Lato";
  font-size: 65px;
  font-weight: 300;
  line-height: normal;
  color: rgba(0, 0, 0, 0.85);
  display: flex;
  margin-bottom: 30px;
}
.description {
  height: 10.49%;
  width: 50.32%;
  display: flex;
  margin-bottom: 29px;
  font-family: "Lato";
  font-size: 24px;
  font-weight: 400;
  line-height: 36px;
  color: rgba(0, 0, 0, 0.85);
}
.description-emphasis-1 {
  font-family: "Lato";
  font-size: 24px;
  font-weight: 400;
  line-height: 36px;
  color: rgba(244, 88, 0, 1);
}
.flex-wrapper-one {
  margin-bottom: 121px;
  display: flex;
  align-items: center;
}
.start-button {
  background-color: rgba(55, 158, 90, 1);
  margin-right: 12px;
  padding: 6px 11px;
  display: flex;
  align-items: center;
}
.start-button-text {
  font-family: "Lato";
  font-size: 16px;
  font-weight: 700;
  line-height: normal;
  color: rgba(255, 255, 255, 1);
  flex: 1;
  align-self: stretch;
  display: flex;
}
.more-button {
  padding: 5px 8px 5px 10px;
  display: flex;
  align-items: center;
  border: 1px solid rgba(0, 0, 0, 0.65);
}
.more-button-text {
  font-family: "Lato";
  font-size: 16px;
  font-weight: 700;
  line-height: normal;
  color: rgba(0, 0, 0, 0.65);
  flex: 1;
  align-self: stretch;
  display: flex;
}
.flex-wrapper-two {
  margin-bottom: 63px;
  display: flex;
  align-items: flex-start;
}
.store-now {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  &:not(:last-of-type) {
    margin-right: 94px;
  }
}
.store-now-icon {
  width: 16.71%;
  height: 25.15%;
  margin-bottom: 19.7px;
}
.store-now-title {
  width: 93.56%;
  height: 19.39%;
  font-family: "Lato";
  font-size: 32px;
  font-weight: 300;
  line-height: normal;
  color: rgba(0, 0, 0, 1);
  margin-bottom: 20px;
}
.store-now-description {
  height: 35.2%;
  font-family: "Lato";
  font-size: 18px;
  font-weight: 400;
  line-height: normal;
  color: rgba(0, 0, 0, 0.75);
  align-self: stretch;
  display: flex;
}
.store-story {
  margin-right: 65px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
.store-story-icon {
  width: 15.22%;
  height: 25.15%;
  margin-bottom: 19.7px;
}
.store-story-title {
  width: 97.22%;
  height: 19.39%;
  font-family: "Lato";
  font-size: 32px;
  font-weight: 300;
  line-height: normal;
  color: rgba(0, 0, 0, 1);
  margin-bottom: 20px;
}
.store-improve-icon {
  width: 14.54%;
  height: 25.15%;
  margin-bottom: 19.7px;
}
.store-improve-title {
  width: 79.94%;
  height: 19.39%;
  font-family: "Lato";
  font-size: 32px;
  font-weight: 300;
  line-height: normal;
  color: rgba(0, 0, 0, 1);
  margin-bottom: 20px;
}
.logo {
  width: 7.23%;
  height: 6.84%;
  margin-left: 1154px;
}
</style>
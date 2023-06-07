<template>
  <div>
    <div class="bg-image2" />
    <h2 id="tiGeo" class="">Acerca de</h2>
    <br />
    <div id="parGeo" class="mb-5">
      <!-- <p class="parrafoGeo">
        Las primeras estaciones acelerométricas (acelerógrafos) a cargo del
        Instituto Geofísico del Perú, funcionaron en los años 40 en el Parque de
        la Reserva y en el campus de la Universidad de La Molina, esta última
        aún operativa, pero con instrumental moderno. En la década de los 80 y
        90, la red acelerométrica estuvo integrada por 17 estaciones , todas con
        registros en papel fotográfico y/o cintas magnéticas. 
      </p>-->
      <p class="parrafoGeo pb-8">
        Red Geofísica Nacional (REDGEN) es la red administrada por el IGP que
        permite el monitoreo y vigilancia de los peligros de origen natural y
        antrópicos asociados con la dinámica interna y externa de la Tierra,
        constituyendo la fuente de información oficial del Estado sobre este
        tipo de peligros para la gestión del riesgo de desastres.
      </p>
      <!--<a id="btnFunci" class="my-linktop" @click="recepFunc">Ver Guia de uso</a>-->
      <br />
      <br />
      <br />
      <br />
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    recepFunc() {
      document.querySelectorAll("#func").forEach((boton) => boton.click());
    },
    recepContac() {
      document.querySelectorAll("#contacto").forEach((boton) => boton.click());
    },
  },
};
</script>

<style>
#tiGeo {
  font-style: normal;
  font-size: 20px;
  line-height: 26px;
  color: #0000Af;
  margin: 0px 0px 0px 45px;
}
#parGeo {
  margin-bottom: 80px !important;
}
.parrafoGeo {
  font-style: normal;
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
  color: #00132e;
  margin-left: 45px;
  margin-right: 45px;
}

.bg-image2 {
  width: 450px;
  height: 370px;
  background-image: linear-gradient(
      to bottom,
      rgba(255, 255, 255, 0) 85%,
      rgba(255, 255, 255, 1) 97%
    ),
    url("https://ide.igp.gob.pe/geovisor/redgen/imagenEstacion.png");
  background-repeat: no-repeat;
  background-size: 100% 100%;
  background-attachment: fixed;
}

::-webkit-scrollbar {
  width: 8px;
  height: 8px;
}

::-webkit-scrollbar-thumb {
  background-color: #bbbbbb;
  border-radius: 5px;
}

::-webkit-scrollbar-thumb:hover {
  background-color: #888;
}
#btnFunci {
  width: 195px;
  height: 41px;
  background: #ffffff;
  border: 1px solid #0000Af;
  color: #0000Af;
  border-radius: 4.26437px;
  cursor: pointer;
  font-weight: 500;
  font-size: 14px;
  line-height: 15px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 45px;
}
#btnFunci:hover {
  background-color: #0000af;
  color: #ffffff;
}
</style>

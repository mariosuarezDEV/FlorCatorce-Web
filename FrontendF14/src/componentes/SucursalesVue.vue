<script>
import InfoSucursalVue from '@/componentes/InfoSucursalVue.vue'

export default {
  data: () => ({}),
  methods: {
    // Define any methods you need here
  },
  components: {
    InfoSucursalVue,
  },
}
</script>

<template>
  <h3 class="fs-1 mb-4">Visitanos ¡Tenemos un espacio para ti!</h3>
  <div class="row">
    <div class="col-md-6 col-12">
      <!-- Sucursal 1 -->
      <InfoSucursalVue
        url="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3760.3559097158177!2d-96.89857912364833!3d19.526327781773254!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85db33cf3560abdd%3A0x801846216e42d70e!2sFlor%20Catorce%20%C3%81nimas!5e0!3m2!1ses-419!2smx!4v1751571878099!5m2!1ses-419!2smx"
        nombre="Sucursal Araucarias"
        direccion="Pico de Orizaba 6, Sipeh Animas, 91067 Xalapa, Veracruz"
      />
    </div>
    <div class="col-md-6 col-12">
      <!-- Sucursal 2 -->
      <InfoSucursalVue
        url="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3760.3871064383557!2d-96.92564072364836!3d19.524987381774274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85db2df8d1b0b4d9%3A0x27f3e9085b9dbcd5!2sFlor%20Catorce%20Centro!5e0!3m2!1ses-419!2smx!4v1751571994897!5m2!1ses-419!2smx"
        nombre="Sucursal Centro"
        direccion="José María Morelos 1, 91090 Xalapa, Veracruz"
      />
    </div>
  </div>
</template>

<style scoped></style>

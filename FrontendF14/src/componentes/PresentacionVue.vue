<script>
import CarruselVue from '@/componentes/CarruselVue.vue';
export default {
  name: 'PresentacionVue',
  data: () => ({

  }),
  methods: {
    // Define any methods you need here
  },
  components: {
    CarruselVue
  },

}
</script>

<template>
  <div class="row justify-content-center align-items-center g-4">
    <div class="col-md-5">
        <h3 class="fs-1">El aroma que despierta tus sentidos</h3>
        <p class="preesentacion">Nuestro espacio está diseñado para que te sientas como en casa, rodeado de un ambiente rústico, cultural y natural.</p>
        <div class="row g-3 text-center">
          <a href="#sucursales" class="btn btn-primary p-2"><i class="fa-solid fa-map-location-dot"></i> Visita nuestras sucursales</a>
          <a href="#productos" class="btn btn-outline-primary p-2"><i class="fa-solid fa-fire"></i> Productos destacados</a>
        </div>
    </div>
    <div class="col-md-7">
        <CarruselVue/>
    </div>
  </div>
</template>

<style scoped>
.preesentacion{
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap');
  font-family: "Playfair Display", serif;
}

</style>

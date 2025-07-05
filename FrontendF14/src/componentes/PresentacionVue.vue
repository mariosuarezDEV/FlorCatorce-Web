<script>
import CarruselVue from '@/componentes/CarruselVue.vue';

export default {
  name: 'PresentacionVue',
  components: {
    CarruselVue
  }
};
</script>

<template>
  <div class="container py-5">
    <div class="row align-items-center g-5">
      <div class="col-md-5 text-center text-md-start">
        <h3 class="display-5 fw-bold mb-3">El aroma que despierta tus sentidos</h3>
        <p class="presentacion lead mb-4">
          Nuestro espacio está diseñado para que te sientas como en casa, rodeado de un ambiente rústico, cultural y natural.
        </p>
        <div class="d-grid gap-3 d-md-block">
          <a href="#sucursales" class="btn btn-primary me-md-3 mb-2 mb-md-0">
            <i class="fa-solid fa-map-location-dot"></i> Visita nuestras sucursales
          </a>
          <a href="#productos" class="btn btn-outline-primary">
            <i class="fa-solid fa-fire"></i> Productos destacados
          </a>
        </div>
      </div>
      <div class="col-md-7">
        <CarruselVue />
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&display=swap');

.presentacion {
  font-family: "Playfair Display", serif;
  color: #4e342e;
}
</style>

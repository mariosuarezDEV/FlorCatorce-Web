<script>
import NavBar from '@/componentes/NavBar.vue'
import PresentacionVue from '@/componentes/PresentacionVue.vue'
import ProductosVue from '@/componentes/ProductosVue.vue'
import SucursalesVue from '@/componentes/SucursalesVue.vue'
import DeliveryGridVue from '@/componentes/DeliveryGridVue.vue'

export default {
  name: 'SingleView',
  data: () => ({}),
  methods: {
    // Define any methods you need here
  },
  components: {
    NavBar,
    PresentacionVue,
    ProductosVue,
    SucursalesVue,
    DeliveryGridVue
  },
}
</script>

<template>
  <NavBar />
  <!-- Imagen de presentacion -->
  <div class="container">
    <div class="row">
      <div class="col-12">
        <PresentacionVue />
      </div>
    </div>
  </div>
  <div class="bg-secondary" id="productos">
    <div class="container">
      <div class="row" data-bs-theme="dark">
        <div class="col-12 mt-5 mb-5">
          <ProductosVue />
        </div>
      </div>
    </div>
  </div>
  <div class="container" id="sucursales">
    <div class="row">
      <div class="col-12 mt-5 pt-5 mb-5 pb-5">
        <SucursalesVue />
      </div>
    </div>
  </div>
  <div class="min-vh-100 position-relative">
    <!-- Capa de imagen de fondo oscurecida -->
    <div class="position-absolute top-0 start-0 w-100 h-100 fondo-imagen" style="z-index: 0;"></div>

    <!-- Capa de superposición con color primario semi-transparente -->
    <div class="position-absolute top-0 start-0 w-100 h-100 bg-primary opacity-75" style="z-index: 1;"></div>

    <!-- Contenido centrado -->
    <div class="position-relative z-2 d-flex justify-content-center align-items-center min-vh-100 text-white text-center" data-bs-theme="dark">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <h3 class="fs-3 mb-4">¡Donde quiera que estes!</h3>
            <img src="../assets/Logo.svg" alt="" class="img-fluid mb-4" style="max-width: 150px;">
            <h3 class="fs-1 mb-4">Flor Catorce</h3>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.fondo-imagen {
  background-image: url('/img/Fondo.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
</style>


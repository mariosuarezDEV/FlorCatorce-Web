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
  <div class="min-vh-100 bg-secondary" id="productos">
    <div class="container">
      <div class="row" data-bs-theme="dark">
        <div class="col-12 mt-5 pt-5">
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
  <div class="container" id="sucursales">
    <div class="row">
      <div class="col-12 mb-5 pb-5">
        <DeliveryGridVue />
      </div>
    </div>
  </div>
</template>

<style scoped></style>

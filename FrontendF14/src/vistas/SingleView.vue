<script>
import NavBar from '@/componentes/NavBar.vue'
import PresentacionVue from '@/componentes/PresentacionVue.vue'
import ProductosVue from '@/componentes/ProductosVue.vue'

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
  },
}
</script>

<template>
  <NavBar />
  <!-- Imagen de presentacion -->
  <div class="container">
    <div class="row">
      <div class="col-12">
        <PresentacionVue/>
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
  <div class="min-vh-100">
    <div class="container">
      <div class="row" data-bs-theme="dark">
        <div class="col-12 mt-5 pt-5">

        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>

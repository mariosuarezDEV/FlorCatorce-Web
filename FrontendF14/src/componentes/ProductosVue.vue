<script>
import GCardVue from '@/componentes/GCardVue.vue'

export default {
  name: 'ProductosVue',
  data: () => ({

  }),
  methods: {
    // Define any methods you need here
  },
  components: {
    GCardVue,
  },
}
</script>

<template>
  <h3 class="fs-1">Los Favoritos</h3>
  <h3 class="fs-3 mb-2">Descubre nuestros productos más populares entre los clientes.</h3>
  <div class="row g-2">
    <div class="col-12">
      <GCardVue/>
    </div>
  </div>
</template>

<style scoped></style>

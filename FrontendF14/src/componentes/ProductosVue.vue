<script>
import CardVue from '@/componentes/CardVue.vue'
import GCardVue from '@/componentes/GCardVue.vue'

export default {
  data: () => ({

  }),
  methods: {
    // Define any methods you need here
  },
  components: {
    CardVue,
    GCardVue,
  },
}
</script>

<template>
  <h3 class="fs-1">Los Favoritos</h3>
  <div class="row g-2">
    <div class="col-12">
      <GCardVue/>
    </div>
    <div class="col-12">
      <GCardVue/>
    </div>
  </div>
</template>

<style scoped></style>

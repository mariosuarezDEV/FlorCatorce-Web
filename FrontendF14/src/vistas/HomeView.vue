<script>
import NavBar from '../componentes/NavBar.vue'
import GaleryVue from '../componentes/GaleryVue.vue'
export default {
  name: 'FlorCatorce',
  data: () => ({

  }),
  components: {
    NavBar,
    GaleryVue
  }
}
</script>

<template>
<NavBar/>
  <div class="">
    <GaleryVue />
  </div>
</template>

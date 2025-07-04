<script>
export default {
  name: 'CardVue',
  data: () => ({
    // Aquí puedes definir propiedades reactivas si es necesario
  }),
  methods: {
    // Aquí puedes definir métodos si es necesario
  },
  components: {
    // Aquí puedes registrar otros componentes si es necesario
  },
  props: {
    // Aquí puedes definir propiedades que se pueden pasar al componente
    img:(
      String
    ),
    title:(
      String
    ),
    description:(
      String
    ),
    fecha_actualizacion:(
      String
    )
  }
}
</script>

<template>
  <div class="card bg-primary">
    <img v-bind:src='img' alt="" class="card-img-top">
    <div class="card-body">
      <h5 class="card-title">{{title}}</h5>
      <p class="card-text">{{description}}</p>
      <p class="card-text"><small class="text-body-secondary">{{fecha_actualizacion}}</small></p>
    </div>
  </div>
</template>

<style scoped>

</style>

<script >
export  default {
  name: 'ButtonVue',
  data: () =>({
    // Data properties can be defined here
  }),
  methods: {

  },
  components: {

  },
  props:{
    // Propiedad que se puede pasar al componente
    url: (
      String
    ),
    nombre: (
      String
    ),
  }
}
</script>

<template>
<!-- SFC (Single File Component --->
<div>
  <img :src='url' alt="Logo VueJS">
  <h2>{{nombre}}</h2>
  <button>Curso de {{nombre}}</button>
</div>
</template>

<style scoped>
div{
  text-align: center;
  display: inline-block;
  padding: 1%;
  margin: 4px;

}

img{
  width: 8rem;
  height: 100px;
  padding: 0.5rem;
}
</style>

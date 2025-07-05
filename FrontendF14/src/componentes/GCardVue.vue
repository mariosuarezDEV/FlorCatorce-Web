<script lang="ts">
import CardVue from '@/componentes/CardVue.vue';

export default {
  name: 'GCardVue',
  components: { CardVue }
};
</script>

<template>
  <div class="row g-4">
    <div class="col-12 col-sm-6 col-lg-4" v-for="(producto, i) in productos" :key="i">
      <CardVue
        :img="producto.img"
        :title="producto.title"
        :description="producto.description"
        :fecha_actualizacion="producto.fecha_actualizacion"
      />
    </div>
  </div>
</template>

<script setup lang="ts">
const productos = [
  {
    img: '/img/BigCrunchQuesadilla.png',
    title: 'Big Crunch Quesadilla',
    description: 'Crujiente tortilla rellena de queso y carne con especias especiales.',
    fecha_actualizacion: 'Hace 3 minutos'
  },
  {
    img: '/img/BrownieHelado.png',
    title: 'Brownie con Helado',
    description: 'Postre caliente con chocolate artesanal y helado casero.',
    fecha_actualizacion: 'Hace 12 minutos'
  },
  {
    img: '/img/LatteGrande.png',
    title: 'Café Especial',
    description: 'Café de grano tostado al momento, con notas florales y especiadas.',
    fecha_actualizacion: 'Hace 1 hora'
  }
];
</script>

<style scoped></style>

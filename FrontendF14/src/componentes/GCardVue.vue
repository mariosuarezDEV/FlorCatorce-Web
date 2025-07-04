<script lang="ts">
import CardVue from '@/componentes/CardVue.vue'

export default {
  name: 'GCardVue',
  components: { CardVue },
}
</script>

<template>
  <div class="card-group">
    <CardVue
      img="/img/BigCrunchQuesadilla.png"
      title="Big Crunch Quesadilla"
      description="Descripción breve del producto. Aquí puedes incluir detalles como ingredientes o características especiales."
      fecha_actualizacion="Ultima vez hace 3 minutos"
    />
    <CardVue
      img="/img/BigCrunchQuesadilla.png"
      title="Big Crunch Quesadilla"
      description="Descripción breve del producto. Aquí puedes incluir detalles como ingredientes o características especiales."
      fecha_actualizacion="Ultima vez hace 3 minutos"
    />
    <CardVue
      img="/img/BigCrunchQuesadilla.png"
      title="Big Crunch Quesadilla"
      description="Descripción breve del producto. Aquí puedes incluir detalles como ingredientes o características especiales."
      fecha_actualizacion="Ultima vez hace 3 minutos"
    />
  </div>
</template>

<style scoped></style>

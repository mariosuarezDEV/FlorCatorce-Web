<script>

</script>

<template>
  <section id="galeria" class="gallery-section container">
    <h2>Nuestra Galería</h2>
    <div class="gallery-grid">
      <div class="gallery-item"><img src="../assets/LatteGrande.png" alt="Toast de Salmon"></div>
      <div class="gallery-item"><img src="../assets/Chilaquiles.png" alt="Chilaquiles Verdes"></div>
      <div class="gallery-item"><img src="../assets/Sandwitch.png" alt="Foto de interior"></div>
      <div class="gallery-item"><img src="../assets/Mezcalate_ChocolateTradicional.png" alt="Foto de evento"></div>
    </div>
  </section>
</template>

<style scoped>
.gallery-section {
  text-align: center;
  padding: 4rem 2rem;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
  margin-top: 2rem;
}

.gallery-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 8px;
  transition: transform 0.3s;
}

.gallery-item img:hover {
  transform: scale(1.05);
}
</style>

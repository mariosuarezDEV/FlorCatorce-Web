<script>
</script>

<template>
  <div id="carouselExample" class="carousel slide carousel-fade" data-bs-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="../assets/ToastSalmon.png" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="../assets/BrownieHelado.png" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="../assets/ChilaquiesVerdes.png" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="../assets/HotCakesAmericanos.png" class="d-block w-100" alt="...">
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</template>

<style scoped>
html, body {
  margin: 0;
  padding: 0;
  overflow: hidden; /* evita el scroll */
  height: 100vh;
}

.carousel,
.carousel-inner,
.carousel-item,
.carousel-item img {
  height: 100vh; /* altura de la ventana */
}

.carousel-item img {
  object-fit: cover; /* para que la imagen se ajuste bien */
  width: 100%;
}
</style>

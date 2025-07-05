<script>
export default {
  name: 'CarruselVue'
};
</script>

<template>
  <div id="carouselExample" class="carousel slide shadow rounded-4 overflow-hidden" data-bs-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="@/assets/img/portada_uno.jpg" class="d-block w-100 img-fluid" alt="Café 1">
      </div>
      <div class="carousel-item">
        <img src="@/assets/img/portada_tres.jpg" class="d-block w-100 img-fluid" alt="Café 2">
      </div>
      <div class="carousel-item">
        <img src="@/assets/img/portada_dos.jpg" class="d-block w-100 img-fluid" alt="Café 3">
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Anterior</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Siguiente</span>
    </button>
  </div>
</template>

<style scoped>
.carousel img {
  object-fit: cover;
  height: 100%;
  max-height: 420px;
}
</style>

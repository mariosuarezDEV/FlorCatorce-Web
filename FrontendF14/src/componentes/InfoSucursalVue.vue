<script>
export default {
  props: {
    url: {
      type: String,
      required: true
    },
    nombre: {
      type: String,
      required: true
    },
    descripcion: {
      type: String,
      default: "Esta es una tarjeta más amplia con texto de apoyo a continuación como introducción natural a contenido adicional."
    },
    ultimaActualizacion: {
      type: String,
      default: "Hace 3 minutos"
    }
  }
}
</script>

<template>
  <div class="card mb-3 shadow-sm hover-shadow bg-primary" data-bs-theme="dark">
    <div class="row g-0">
      <div class="col-md-4">
        <iframe
          :src="url"
          class="img-fluid rounded-start h-100 w-100"
          title="Contenido multimedia"
          allowfullscreen
          loading="lazy"
        ></iframe>
      </div>
      <div class="col-md-8 d-flex flex-column">
        <div class="card-body">
          <h5 class="card-title fw-bold fs-3">{{nombre}}</h5>
          <p class="card-text text-muted">{{descripcion}}</p>
          <div class="">
            <a href="http://" class="card-text fs-4 btn btn-secondary m-2"><i class="fa-brands fa-whatsapp"></i></a>
            <a href="http://" class="card-text fs-4 btn btn-secondary m-2"><i class="fa-solid fa-phone"></i></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.hover-shadow:hover {
  box-shadow: 0 .5rem 1rem rgba(0,0,0,.15)!important;
  transition: box-shadow 0.2s ease;
}

/* Mejorar la relación de aspecto del iframe */
.rounded-start {
  aspect-ratio: 16 / 9;
  object-fit: cover;
}
</style>

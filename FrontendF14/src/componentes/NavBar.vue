<script></script>

<template>
  <nav class="navbar navbar-expand-lg bg-primary sticky-top shadow-sm" data-bs-theme="dark">
    <div class="container-fluid">
      <a class="navbar-brand d-flex align-items-center justify-content-center empresa_text p-2" href="#">
        <img src="../assets/Logo.svg" alt="Logo" width="30" height="24" class="justify-content-center" />
        Flor Catorce
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#"><i class="fa-solid fa-house"></i> Inicio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" href="#"><i class="fa-solid fa-map-location-dot"></i> Sucursales</a>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle active"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              <i class="fa-solid fa-utensils"></i> Delivery
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#">Plick</a></li>
              <li><a class="dropdown-item" href="#">Uber Eats</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap');
.empresa_text{
  font-family: "Playfair Display", serif;
}
</style>

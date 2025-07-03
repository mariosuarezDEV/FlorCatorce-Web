<script>

</script>

<template>
  <header class="main-header">
    <div class="container">
      <div class="logo">
        <img src="../assets/Logo.svg" alt="Logo Cafetería">
        <span>Flor Catorce</span>
      </div>
      <nav>
        <a href="#">Inicio</a>
        <a href="#nosotros">Nosotros</a>
        <a href="#galeria">Galería</a>
        <a href="#contacto">Contacto</a>
      </nav>
    </div>
  </header>
</template>

<style scoped>
.main-header {
  background-color: var(--cafe-oscuro);
  color: var(--blanco-hueso);
  padding: 1rem 0;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}

.main-header .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  display: flex;
  align-items: center;
  font-size: 1.5rem;
  font-family: 'Playfair Display', serif;
}

.logo img {
  height: 40px;
  margin-right: 10px;
}

nav a {
  color: var(--blanco-hueso);
  margin-left: 20px;
  font-size: 1.1rem;
  transition: color 0.3s;
}

nav a:hover {
  color: var(--verde-hoja);
}

@media (max-width: 768px) {
  .main-header .container {
    flex-direction: column;
  }
  nav {
    margin-top: 1rem;
  }
}
</style>

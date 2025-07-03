<script>

</script>

<template>
  <section class="hero-section" id="inicio">
    <div class="hero-content">
      <h1>El aroma que despierta tus sentidos</h1>
      <p>Café de especialidad y platillos hechos con el corazón.</p>
      <div class="button-container">
        <a href="https://menu.plick.app/directorio/florcatorcesucursales" target="_blank" class="cta-button">Menú de Plick</a>
        <a href="https://www.ubereats.com/mx/store/flor-catorce-araucarias/Ai58KTR7W_exzeLUzPcWHA?srsltid=AfmBOopzvK1gvhQvqHlncC7vp63U_tDNw2bxn7_NDtyB0CHOqe4qXvl0" target="_blank" class="cta-button secondary">Menú de Uber</a>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Asumiendo que estos colores están en tu CSS global (styles.css) */
:root {
  --cafe-oscuro: #3E2723;
  --cafe-claro: #A1887F;
  --verde-hoja: #4CAF50;
  --blanco-hueso: #F5F5F5;
}

.hero-section {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('@/assets/Fondo.jpg');
  height: 90vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: var(--blanco-hueso);
}

.hero-content h1 {
  font-size: 3.5rem;
  margin-bottom: 1rem;
  color: var(--blanco-hueso);
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); /* Sombra para resaltar el texto */
}

.hero-content p {
  font-size: 1.5rem;
  margin-bottom: 2.5rem; /* Aumentamos el margen inferior */
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5); /* Sombra ligera */
}

.button-container {
  display: flex;
  justify-content: center;
  gap: 20px; /* Espacio entre los botones */
  flex-wrap: wrap; /* Para que se ajusten en móviles */
}

/* --- NUEVOS ESTILOS PARA LOS BOTONES --- */

.cta-button {
  padding: 15px 35px;
  border-radius: 50px; /* Bordes más redondeados para un look moderno */
  font-size: 1.2rem;
  font-weight: bold; /* Texto en negrita */
  text-transform: uppercase; /* Mayúsculas para un estilo más fuerte */
  letter-spacing: 1px; /* Espaciado entre letras */
  border: 2px solid transparent; /* Borde base transparente */
  transition: all 0.3s ease; /* Transición suave para todos los efectos */
  cursor: pointer;
  display: inline-block; /* Asegura que se apliquen bien los estilos */
}

/* Estilo del botón principal (Plick) */
.cta-button {
  background-color: var(--cafe-claro);
  color: var(--cafe-oscuro);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}

/* Estilo del botón secundario (Uber) */
.cta-button.secondary {
  background-color: transparent;
  border-color: var(--cafe-claro);
  color: var(--cafe-claro);
  box-shadow: none; /* Sin sombra inicial */
}

/* --- EFECTOS HOVER --- */

/* Hover para el botón principal */
.cta-button:hover {
  transform: translateY(-3px); /* Se eleva un poco */
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.3);
  background-color: #b9a096; /* Un tono ligeramente más claro de café */
}

/* Hover para el botón secundario */
.cta-button.secondary:hover {
  background-color: var(--cafe-claro);
  color: var(--cafe-oscuro);
  transform: translateY(-3px);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}


@media (max-width: 768px) {
  .hero-content h1 {
    font-size: 2.5rem;
  }
  .hero-content p {
    font-size: 1.2rem;
  }
  .button-container {
    flex-direction: column; /* Apila los botones verticalmente */
    align-items: center;
    gap: 15px;
  }
  .cta-button {
    width: 80%;
    max-width: 300px;
  }
}
</style>

<script>

</script>

<template>
  <section id="nosotros" class="about-section">
    <div class="container about-flex">
      <div class="about-text">
        <h2>Un Rincón con Historia y Sabor</h2>
        <p>Somos más que una cafetería, somos un punto de encuentro para amantes del buen café y la comida auténtica. Nuestro espacio está diseñado para que te sientas como en casa, rodeado de un ambiente rústico, cultural y natural.</p>
        <p>Cada grano de café y cada ingrediente son seleccionados cuidadosamente para ofrecerte una experiencia inolvidable.</p>
      </div>
      <div class="about-image">
        <img src="../assets/FlorPortada.jpg" alt="Interior del café con plantas">
      </div>
    </div>
  </section>
</template>

<style scoped>
.about-section {
  background-color: var(--cafe-claro);
  color: var(--blanco-hueso);
  padding: 4rem 0;
}

.about-flex {
  display: flex;
  align-items: center;
  gap: 3rem;
}

.about-text {
  flex: 1;
}

.about-text h2 {
  color: var(--blanco-hueso);
}

.about-image {
  flex: 1;
}

.about-image img {
  max-width: 100%;
  border-radius: 8px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

@media (max-width: 768px) {
  .about-flex {
    flex-direction: column;
  }
}
</style>

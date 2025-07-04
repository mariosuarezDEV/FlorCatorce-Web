<script>

</script>

<template>
  <section id="contacto" class="contact-section">
    <div class="container contact-flex">
      <div class="contact-info">
        <h2>Sucursal Centro</h2>
        <p><strong>Dirección:</strong> José María Morelos 1, 91090 Xalapa, Veracruz</p>
        <p><strong>Teléfono:</strong> 228 132 5126</p>
        <p><strong>Horario:</strong> Lunes a Domingo de 9:00 a 21:00 hrs.</p>
      </div>
      <div class="contact-map">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3760.3871064383557!2d-96.92564072364836!3d19.524987381774274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85db2df8d1b0b4d9%3A0x27f3e9085b9dbcd5!2sFlor%20Catorce%20Centro!5e0!3m2!1ses-419!2smx!4v1751571994897!5m2!1ses-419!2smx"
          width="100%"
          height="350"
          style="border:0;"
          allowfullscreen=""
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade">
        </iframe>
      </div>
    </div>
  </section>

  <section id="contacto" class="contact-section">
    <div class="container contact-flex">
      <div class="contact-info">
        <h2>Sucursal Araucarias</h2>
        <p><strong>Dirección:</strong> Pico de Orizaba 6, Sipeh Animas, 91067 Xalapa, Veracruz</p>
        <p><strong>Teléfono:</strong> 228 354 9526</p>
        <p><strong>Horario:</strong> Lunes a Domingo de 9:00 a 21:00 hrs.</p>
      </div>
      <div class="contact-map">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3760.3559097158177!2d-96.89857912364833!3d19.526327781773254!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85db33cf3560abdd%3A0x801846216e42d70e!2sFlor%20Catorce%20%C3%81nimas!5e0!3m2!1ses-419!2smx!4v1751571878099!5m2!1ses-419!2smx"
          width="100%"
          height="350"
          style="border:0;"
          allowfullscreen=""
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade">
        </iframe>
      </div>
    </div>
  </section>
</template>

<style scoped>
.contact-section {
  background-color: var(--blanco-hueso);
  padding: 4rem 0;
}

.contact-flex {
  display: flex;
  gap: 2rem;
  align-items: center;
}

.contact-info {
  flex: 1;
}

.contact-map {
  flex: 1.5;
  border-radius: 8px;
  overflow: hidden;
}

@media (max-width: 768px) {
  .contact-flex {
    flex-direction: column;
  }
}
</style>

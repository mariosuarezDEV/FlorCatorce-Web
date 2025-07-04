<script>

</script>

<template>
  <section id="menu" class="menu-section container">
    <h2>Nuestro Menú</h2>
    <div class="menu-grid">
      <div class="menu-item" v-for="item in menu" :key="item.nombre">
        <img :src="require(`@/assets/images/${item.img}`)" :alt="item.nombre">
        <h3>{{ item.nombre }}</h3>
        <p>{{ item.descripcion }}</p>
        <span class="price">{{ item.precio }}</span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      menu: [
        { nombre: 'Café Americano', descripcion: 'Grano seleccionado de las altas montañas.', precio: '$45.00', img: 'plato1.jpg' },
        { nombre: 'Chilaquiles Verdes', descripcion: 'Con pollo, queso fresco, crema y cebolla.', precio: '$120.00', img: 'plato2.jpg' },
        { nombre: 'Pastel de Chocolate', descripcion: 'Hecho con cacao orgánico de la región.', precio: '$85.00', img: 'planta1.jpg' }
      ]
    };
  }
};
</script>

<style scoped>
.menu-section {
  text-align: center;
  padding: 4rem 2rem;
}

.menu-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin-top: 2rem;
}

.menu-item {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  padding: 1.5rem;
  transition: transform 0.3s;
}

.menu-item:hover {
  transform: translateY(-10px);
}

.menu-item img {
  max-width: 100%;
  border-radius: 5px;
  margin-bottom: 1rem;
}

.menu-item h3 {
  color: var(--cafe-oscuro);
}

.price {
  display: block;
  margin-top: 1rem;
  font-weight: bold;
  font-size: 1.2rem;
  color: var(--verde-hoja);
}
</style>

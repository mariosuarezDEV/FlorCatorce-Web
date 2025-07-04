<script>
/* import Card from '../componentes/ButtonVue.vue'
import NavBar from '@/componentes/NavBar.vue'
export default {
  data: () => ({
    // Funcion  llave que retorna objetos javascript al template
    empresa: 'Flor Catorce',
    contador: 0,
    nombre: "",
    edad: 0,
    correo: ""
  }),
  methods: {
    // Funciones que se pueden llamar desde el template
    test() {
      console.log('El metodo funciona correctamente')
    },
    incrementar() {
      this.contador++
    },
    decrementar() {
      this.contador--
    },
    resetear() {
      this.contador = 0
    },
    backend() {
      console.log('Nombre:', this.nombre, 'Edad:', this.edad, 'Correo:', this.correo);
    },
  },
  components: {
    // Componentes que se pueden usar en el template
    Card,
    NavBar
  },
} */
</script>

<template>
  <NavBar />
  <div class="emblema">
    <img src="../assets/LogoFlorCatorce.png" alt="Logo de Flor Catorce" class="logo" />
    <h1 class="empresa" v-on:click="test">{{ empresa }}</h1>
  </div>

  <div class="curso">
    <h1>Valor del contador: {{ contador }}</h1>
    <button @click="incrementar()">Subir +1</button>
    <button @click="decrementar()">Bajar +1</button>
    <button @click="resetear()">Resetear</button>
    <p v-show="contador > 10">Estas arriba del numero 10, el numero actual es {{contador}}</p>
    <ul>
      <li v-for="(numero, index) in contador" :key="index">{{index+1}}</li>
    </ul>
  </div>

  <div>
    <Card
      url="https://cdn.svgporn.com/logos/vue.svg?response-content-disposition=attachment%3Bfilename%3Dvue.svg"
      nombre="Vue JS"
    />
    <Card
      url="https://cdn.svgporn.com/logos/django-icon.svg?response-content-disposition=attachment%3Bfilename%3Ddjango-icon.svg"
      nombre="Django"
    />
    <Card
      url="https://cdn.svgporn.com/logos/docker-icon.svg?response-content-disposition=attachment%3Bfilename%3Ddocker-icon.svg"
      nombre="Docker"
    />
    <Card
      url="https://cdn.svgporn.com/logos/python.svg?response-content-disposition=attachment%3Bfilename%3Dpython.svg"
      nombre="Python"
    />
    <Card
      url="https://cdn.svgporn.com/logos/javascript.svg?response-content-disposition=attachment%3Bfilename%3Djavascript.svg"
      nombre="JavaScript"
    />
    <Card
      url="https://cdn.svgporn.com/logos/postgresql.svg?response-content-disposition=attachment%3Bfilename%3Dpostgresql.svg"
      nombre="PostgreSQL"
    />
    <Card
      url="https://cdn.svgporn.com/logos/mysql-icon.svg?response-content-disposition=attachment%3Bfilename%3Dmysql-icon.svg"
      nombre="MySQL"
    />
    <Card
      url="https://cdn.svgporn.com/logos/mongodb-icon.svg?response-content-disposition=attachment%3Bfilename%3Dmongodb-icon.svg"
      nombre="MongoDB"
    />
    <Card
      url="https://cdn.svgporn.com/logos/postman-icon.svg?response-content-disposition=attachment%3Bfilename%3Dpostman-icon.svg"
      nombre="Postman"
    />
    <Card
      url="https://cdn.svgporn.com/logos/htmx-icon.svg?response-content-disposition=attachment%3Bfilename%3Dhtmx-icon.svg"
      nombre="htmx"
    />
    <Card
      url="https://cdn.svgporn.com/logos/bootstrap.svg?response-content-disposition=attachment%3Bfilename%3Dbootstrap.svg"
      nombre="Bootstrap"
    />
    <Card
      url="https://cdn.svgporn.com/logos/debian.svg?response-content-disposition=attachment%3Bfilename%3Ddebian.svg"
      nombre="Debian"
    />
    <Card
      url="https://cdn.svgporn.com/logos/strapi-icon.svg?response-content-disposition=attachment%3Bfilename%3Dstrapi-icon.svg"
      nombre="Strapi"
    />
    <Card
      url="https://cdn.svgporn.com/logos/git-icon.svg?response-content-disposition=attachment%3Bfilename%3Dgit-icon.svg"
      nombre="Git"
    />
  </div>
  <!-- Formularios -->
  <div>
    <form v-on:submit.prevent="backend">
      <label>
        Nombre: <input type="text" required v-model="nombre" />
      </label>

      <label>
        Edad: <input type="number" v-model="edad" />
      </label>

      <label>
        Correo: <input type="email" v-model="correo" />
      </label>

      <button type="submit">Enviar</button>
    </form>
  </div>
  <br>
  <hr />
  <h3>Instalacion de bootstrap</h3>
</template>

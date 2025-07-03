<template>
  <div id="app">
    <TheHeader />
    <main>
      <TheHero />
      <TheAbout />
      <TheGallery />
      <TheContact />
    </main>
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from '@/componentes/TheHeader.vue';
import TheHero from '@/componentes/TheHero.vue';
import TheMenu from '@/componentes/TheMenu.vue';
import TheAbout from '@/componentes/TheAbout.vue';
import TheGallery from '@/componentes/TheGallery.vue';
import TheContact from '@/componentes/TheContact.vue';
import TheFooter from '@/componentes/TheFooter.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheHero,
    TheMenu,
    TheAbout,
    TheGallery,
    TheContact,
    TheFooter

  }
};
</script>

<style>


#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

main {
  flex-grow: 1;
}
</style>

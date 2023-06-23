<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Nav from './components/Nav.Vue'
import Footer from './components/Footer.vue'

</script>

<template>
  <header>
    <Nav></Nav>
  </header>
  <body>
    <RouterView />
    <Footer/>
  </body>
</template>

<style scoped>

</style>

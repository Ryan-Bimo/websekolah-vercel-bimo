<script setup>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
</script>
 
<template>
  <Navbar />
  <RouterView />
  <Footer />
</template>

<style scoped>
  /* CSS khusus buat component ini saja, tidak bocor ke component lain */
</style>
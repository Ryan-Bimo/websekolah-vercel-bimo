<script setup>
const tahun = new Date().getFullYear()
</script>
 
<template>
  <hr />
  <div class="container">
  <footer>
    <medium>&copy; {{ tahun }} RyanBimo — Onlineshop 
Milik Bimo</medium>
  </footer>
  </div>
</template>

<style scoped>
.container {
  color: gray;
  font-family: 'Segoe UI', sans-serif;
  font-weight: bold;
  justify-content: center;
  display: flex;
}
</style>
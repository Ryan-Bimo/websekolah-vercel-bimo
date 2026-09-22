<script setup>
import ContactCard from '../components/ContactCard.vue'
</script>

<template>
<div class="kotak">
     <h1>Hubungi Kami</h1>
</div>

<ContactCard/>
</template>

<style scoped>
.kotak {
  color: white;
  width: 100%;
  height: 100px;
  background: linear-gradient(to bottom, #4e7eb4, #3b588d);
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.4);
  overflow: hidden;
  margin: 15px;
  padding: px;
  text-align: center;
}
</style>
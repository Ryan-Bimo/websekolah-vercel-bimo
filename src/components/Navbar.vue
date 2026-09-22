<template>
  <div class="atas">
  <nav>
    <h2>Ryan Bimo - Onlineshop</h2>
    <RouterLink to="/">Landing</RouterLink> |
    <RouterLink to="/product">Product</RouterLink> |
    <RouterLink to="/about">About</RouterLink> |
    <RouterLink to="/contact">Contact</RouterLink>
  </nav>
  <hr />
  </div>
</template>
 
<script setup>
import { RouterLink } from 'vue-router';

  // JavaScript-nya di sini
</script>
 
<style scoped>
  /* CSS khusus buat component ini saja, tidak bocor ke component lain */
  .atas {
    font-weight: bold;
     font-family: 'Segoe UI', sans-serif;
    color: rgb(231, 240, 250);
    background-color: rgba(46, 134, 83, 0.993);
    border-radius: 10px;
    padding: 5px;
    text-align: center;
  }
</style>
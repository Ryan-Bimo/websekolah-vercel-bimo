<script setup>
defineProps(['gambar', 'h1', 'h2'])
</script>

<template>
 <div class="card">
   <div class="icon"><p>{{ gambar }}</p></div> 
    <h1>{{ h1 }}</h1> 
    <p>{{ h2 }}</p> 
    </div>
</template>

<style scoped>

.card {
  font-family: 'Segoe UI', sans-serif;
  color: black;
  width: 280px;
  background-color: white;
  border: 1px solid black;
  border-radius: 10px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.4);
  overflow: hidden;
  margin: 15px;
  padding: 24px;
  text-align: center;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.card:hover {
transform: translateY(-5px);
}

.icon{
font-size: 2.5rem;
margin-bottom: 16px;
}

</style>
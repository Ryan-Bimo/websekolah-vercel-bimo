<script setup>
defineProps(['h1', 'h2', 'p'])
</script>

<template>
 <div class="card">
   <div class="icon"><p>{{ h1 }}</p></div> 
    <h1>{{ h2 }}</h1> 
    <p>{{ p }}</p> 
    </div>
</template>

<style scoped>

.card {
  font-family: 'Segoe UI', sans-serif;
  color: black;
  background-color: white;
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

.h1 h2{
font-weight: 700;
}

.icon{
font-weight: 700;
color: white;
width: 100px;
height: 100px;
border-radius: 50px;
background: linear-gradient(to bottom, #4e7eb4, #3b588d);
font-size: 2.5rem;
margin-bottom: 16px;
display: flex;
justify-content: center;
align-items: center;
}

</style>
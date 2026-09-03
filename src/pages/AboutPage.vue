<script setup>
import TeamCard from '../components/TeamCard.vue';
</script>

<template> 
  <main> 
    <div class="kotak">
     <h1>Tentang Kami</h1>
</div>

<TeamCard/>

    <!-- <video controls width="480" muted loop> 
      <source src="/video/promo-toko.mp4" type="video/mp4" /> 
      Browser kamu tidak mendukung pemutaran video. 
    </video>  -->
  </main> 
</template> 
  
<style scoped> 
/* video { 
  margin-top: 16px; 
  border-radius: 10px; 
  display: block; 
}  */

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
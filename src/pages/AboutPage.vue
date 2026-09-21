<script setup>
import AboutCard from '../components/AboutCard.vue'
import TeamCard from '../components/TeamCard.vue'

const daftarteam = [
  { id: 1, h1: 'R',
   h2: 'Ryan', p: 'Ketua tim' },
   { id: 2, h1: 'B',
   h2: 'Bimo', p: 'Design UI/UX' },
   { id: 3, h1: 'A',
   h2: 'Adietyo', p: 'Pengembang' },
]
</script>

<template> 
  <main> 
    <div class="kotak">
     <h1>Tentang Kami</h1>
</div>

<AboutCard/>
<div class="container">
  <h1>Tim Kami</h1>
  <TeamCard
       v-for="team in daftarteam"
        :key="team.id"
        :h1="team.h1"
        :h2="team.h2"
        :p="team.p"
      />
      </div>
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

.container {
  font-family: 'Segoe UI', sans-serif;
  display: flex;
  gap: 20px;
  place-content: center;
  flex-wrap: wrap;
}

.container h1{
    background: linear-gradient(to bottom, #4e7eb4, #3b588d);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 10px;
    text-align: center;
    width: 100%;

}

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
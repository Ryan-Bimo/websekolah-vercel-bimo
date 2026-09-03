<script setup>
import LandingCard from '../components/LandingCard.vue'
import PropotitionCard from '../components/PropotitionCard.vue'

const daftarPropotition = [
  { id: 1, gambar: '👔',
   h1: 'Kualitas Terjamin', h2: 'Bahan di pilih langsung dengan kualitas terbaik' },
   { id: 2, gambar: '💰',
   h1: 'Harga Bersahabat', h2: 'Cocok untuk dana pelajar' },
   { id: 3, gambar: '🚛',
   h1: 'Free Ongkir', h2: 'Tidak perlu bayar ongkir, di jamin sampe ke depan rumah' },
]
</script>

<template>
  <main>
    <LandingCard/>
    <div class="container">
      <PropotitionCard
       v-for="propotition in daftarPropotition"
        :key="propotition.id"
        :gambar="propotition.gambar"
        :h1="propotition.h1"
        :h2="propotition.h2"
      />
    </div>
  </main>
</template>

<style scoped>
.container {
  display: flex;
  gap: 20px;
  place-content: center;
  flex-wrap: wrap;
}
</style>
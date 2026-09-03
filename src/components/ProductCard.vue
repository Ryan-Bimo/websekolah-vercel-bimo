<!-- <script setup>
defineProps(['nama', 'harga', 'gambar'])
</script>
 
<template>
  <div class="card">
    <img :src="gambar" :alt="nama" />
    <h3>{{ nama }}</h3>
    <p>Rp {{ harga.toLocaleString('id-ID') }}</p>
    <button class="button">Beli Sekarang</button>
  </div>
</template>
 
<style scoped>
.card {
  border: 1px solid #ddd;
  border-radius: 10px;
  padding: 14px;
  width: 200px;
  text-align: center;
  background-color: white;
}
  .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
        }
.button {
            padding: 10px 15px;
            background: blue;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
}
</style> -->

<script setup> 
import { ref } from 'vue' 
  
defineProps(['nama', 'harga', 'gambar']) 
  
const gambarDipilih = ref(null) 
  
function bukaPreview(src) { 
  gambarDipilih.value = src 
} 
  
function tutupPreview() { 
  gambarDipilih.value = null 
} 

function tambahKeKeranjang(nama) { 
  const suara = new Audio('/audio/notifikasi.mp3') 
  suara.play() 
  alert(`${nama} ditambahkan ke keranjang!`) 
} 
</script> 
  
<template> 
  <div class="card"> 
    <img :src="gambar" :alt="nama" @click="bukaPreview(gambar)" /> 
    <h3>{{ nama }}</h3> 
    <p>Rp {{ harga.toLocaleString('id-ID') }}</p> 
     <button class="button">Beli Sekarang</button>
      <button @click="tambahKeKeranjang(nama)" class="krjg">Tambah ke Keranjang</button> 
  </div> 
  
  <div v-if="gambarDipilih" class="preview-overlay"> 
    <img :src="gambarDipilih" class="preview-besar" /> 
    <button @click="tutupPreview" class="tutup">Tutup</button>
  </div> 
</template> 
  
<style scoped> 
.card { 
  border: 1px solid #ddd; 
  border-radius: 10px; 
  padding: 14px; 
  width: 200px; 
  text-align: center; 
} 
.card img {  width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
           } 

           .button {
            padding: 10px 15px;
            background: blue;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
}

.krjg {
            margin: 10px;
            padding: 10px 15px;
            background: rgb(255, 17, 0);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
}

.tutup{
            margin: 10px;
            padding: 10px 15px;
            background: rgb(10, 10, 10);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
}
  
.preview-overlay { 
  position: fixed; top: 0; left: 0; width: 100%; height: 100%; 
  background: rgba(0, 0, 0, 0.7); 
  display: flex; align-items: center; justify-content: center; 
  cursor: zoom-out; 
} 
.preview-besar { max-width: 80%; max-height: 80%; border-radius: 8px; } 
</style>
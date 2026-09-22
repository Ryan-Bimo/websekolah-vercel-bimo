<script setup>
import { ref } from 'vue'

const nama = ref('')
const email = ref('')
const pesan = ref('')
</script>

<template>
    <div class="kolom">
    <div class="teks">
        <h1>Info Kami</h1>
        <h2>📍 Alamat</h2>
        <p>Sanggar Indah Banjaran Jl.Lengkeng no.12</p>

         <h2>☎ Telepon</h2>
        <p>0895123498765</p>

         <h2>✉ Email</h2>
        <p>onlineshop@ryanbimo.sch.id</p>


    </div>
    <div class="teks">
        <h1>Kirim Pesan</h1>

    <div class="form">
        <label for="nama">Nama</label>
      <br>
      <input id="nama" type="text" v-model="nama" placeholder="Masukkan nama..." />
    </div>
<br>
    <div class="form">
        <label for="email">Email</label>
      <br>
      <input id="email" type="text" v-model="email" placeholder="Masukkan email..." />
    </div>
<br>
    <div class="form">
        <label for="pesan">Pesan</label>
      <br>
      <textarea id="pesan" type="text" v-model="pesan" placeholder="Masukkan pesan..."></textarea>
    </div>

<button class="krjg">KIRIM</button>

    </div>
    </div>
</template>

<style scoped>

.krjg {
    font-weight: bold;
    font-size: 15px;
    width: 100px;
    height: auto;
            margin-top: 40px;
            padding: 10px 15px;
            background: linear-gradient(to bottom, #4e7eb4, #3b588d);
            color: white;
            border: none;
            border-radius: 20px;
            cursor: pointer;
}

.form{
   
    font-weight: bold;
    font-size: 20px;
    background: black;
    -webkit-background-clip: text;
    background-clip: text;
}

.form input{
    border: black;
    margin-top: 10px;
    padding: 5px;
    border-radius: 10px;
    width: 250px;
    height: 30px;
}

.form textarea{
    border: black;
    margin-top: 10px;
    padding: 5px;
    border-radius: 10px;
    width: 250px;
    height: 30px;
}

.kolom{
font-family: 'Segoe UI', sans-serif;
display: flex; 
align-items: flex-start;
margin: 50px;
flex: 1;
flex-direction: row;
overflow: hidden;
}

.teks {
    flex: 1;
}

.teks h1{
    background: linear-gradient(to bottom, #4e7eb4, #3b588d);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 50px;
}

.teks h2{
    font-weight: bold;
    font-size: 20px;
    margin-bottom: -20px;
}

.teks p{
    margin-left: 20px;
}
</style>
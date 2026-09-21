<template>
<div class="kolom">
    <div class="teks">
        <h1>Cerita Kami</h1>
    <p>Online Shop ini merupakan sebuah website toko online yang dikembangkan sebagai bagian dari proyek pembelajaran siswa SMK YADIKA SOREANG. Website ini dibuat oleh Ryan Bimo sebagai sarana untuk menerapkan keterampilan dalam bidang teknologi, khususnya pengembangan website dan sistem informasi.
Melalui proyek ini, Ryan Bimo mengembangkan sebuah platform online shop yang sederhana, modern, dan mudah digunakan. Website ini dirancang untuk memberikan pengalaman berbelanja yang praktis sekaligus menjadi wadah bagi siswa untuk mengembangkan kreativitas dan kemampuan di dunia teknologi.
Proses pengembangan website ini menjadi pengalaman berharga dalam mempelajari bagaimana sebuah website dibangun, mulai dari perancangan tampilan, pengelolaan produk, hingga penerapan fitur-fitur yang mendukung aktivitas jual beli secara online.
</p>
<p>Kami berharap online shop ini tidak hanya menjadi sebuah proyek sekolah, tetapi juga menjadi langkah awal untuk terus berkarya, belajar, dan mengembangkan kemampuan di bidang teknologi digital.</p>
    </div>
    <div class="gambar">
        <img src="/gambar/toko-bimo.png" alt="Toko Online">
    </div>
</div>
</template>

<style scoped>
.kolom{
display: flex; 
align-items: flex-start;
margin: 50px;
flex: 1;
flex-direction: row;
overflow: hidden;
}

.gambar img{
 width: 600px;
 height: auto;
 border-radius: 10px;
}

.teks {
    flex: 1;
}

.teks h1{
    background: linear-gradient(to bottom, #4e7eb4, #3b588d);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 10px;
}

.teks p{
    margin-top: 0;
}
</style>
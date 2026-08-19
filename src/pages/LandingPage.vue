<template>
  <main>
<div class="judul">
  <h2>Selamat Datang di Toko Online SMK Yadika Soreang</h2>
  <p>Temukan berbagai produk menarik dan berkualitas di sini. Jelajahi koleksi
  kami dan temukan penawaran terbaik untuk kebutuhan Anda.</p>
  <button class="button1"><RouterLink to="/product">Shop Now</RouterLink></button>
</div>

<div class="container">
  <div class="card">
    <p>🏆</p>
    <h3>Kualitas Papan Atas</h3>
    <p>sekolah ini sangat bagus dan  mantap</p>
  </div>
  <div class="card">
    <p>💳</p>
    <h3>Pembayaran Mudah</h3>
    <p>Pembayaran bisa COD dan Via Transfer</p> 
  </div>
</div>
<div class="container">
<div class="card">
  <p>🚚</p>
  <h3>Restock sampai kiamat</h3>
  <p>Anti Pre-Order.</p>
</div>
</div>

  </main>
</template>

<style scoped>

  .judul { 
  border: 1px solid #ddd; 
  border-radius: 10px; 
  padding: 14px; 
  background: linear-gradient(to right, #2E75B6, #4A90E2);
  text-align: center; 
  color: white;
} 
.card { 
  border: 1px solid #020000; 
  border-radius: 10px; 
  padding: 16px; 
  width: 200px; 
  text-align: center;
  color: rgb(0, 0, 0);
  margin-top: 10px;
  margin-bottom: 10px;
  margin-left: 10px;
} 

.card:hover {
  transform: scale(1.05);
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 100px;
  margin-right: 100px;
}
.button1 {
   background: linear-gradient(to right, #f7f8f8, #fcfdfd56);
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 999px;
}
</style>
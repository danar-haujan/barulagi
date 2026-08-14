<script setup>
import ProductCard from '../components/ProductCard.vue'
 
const daftarProduk = [
  { id: 1, nama: 'James Boogie', harga: 75000, gambar: 
'https://placehold.co/150' },
  { id: 2, nama: 'Tracktop Adidas', harga: 35000, gambar: 
'https://placehold.co/150' },
  { id: 3, nama: 'Sepatu', harga: 120000, gambar: 
'https://placehold.co/150' },
]
</script>
 
<template>
  <main>
    <h1 class="txt">Produk Kami</h1>
    <div class="grid">
      <ProductCard
        v-for="produk in daftarProduk"
        :key="produk.id"
        :nama="produk.nama"
        :harga="produk.harga"
        :gambar="produk.gambar"
      />
    </div>
  </main>
</template>
 
<style scoped>
.grid {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
}
</style>
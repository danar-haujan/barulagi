<script setup>
import ProductCard from '../components/ProductCard.vue'
 
const daftarProduk = [
  { id: 1, nama: 'Belanja', harga: 75000, gambar: '/images/mengbelanja.jpg' },
  { id: 2, nama: 'Adalah', harga: 35000, gambar: '/images/rusidmarah.jpg' },
  { id: 3, nama: 'Kopdes', harga: 120000, gambar: '/images/kopdes.jpg' },
]

</script>
 
<template>
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 p-6">
    <ProductCard
      v-for="produk in daftarProduk"
      :key="produk.id"
      :nama="produk.nama"
      :harga="produk.harga"
      :gambar="produk.gambar"
    />
  </div>
</template>
 
<style scoped>
.grid {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
}
</style>
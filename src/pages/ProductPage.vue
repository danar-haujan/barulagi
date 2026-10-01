<script setup>
import ProductCard from '../components/ProductCard.vue'
 
const daftarProduk = [
  { id: 1, nama: 'AFFILICTION', harga: 1750000, gambar: '/images/affi.jpg' },
  { id: 2, nama: 'TAPOUT', harga: 3500000, gambar: '/images/tapout.jpg' },
  { id: 3, nama: 'TAPOUT', harga: 1500000, gambar: '/images/tapout2.jpg' },
  { id: 4, nama: 'AFFILICTION', harga: 1200000, gambar: '/images/images.jpg' },
  { id: 5, nama: 'AFFILICTION', harga: 1000000, gambar: '/images/pantekl.jpg' },
  { id: 6, nama: 'PHB', harga: 10000000000000000000, gambar: '/images/phb.jpg' },
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
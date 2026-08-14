<script setup>
import TeamCard from '../components/TeamCard.vue'
import fotoCerita from '../assets/abot.png'

const daftarTim = [
  {
    nama: 'rusdi',
    jabatan: 'Ketua Kelompok'
  },
  {
    nama: 'Budi',
    jabatan: 'Anggota'
  },
  {
    nama: 'Si Imut',
    jabatan: 'Anggota'
  }
]
</script>

<template>
  <main>
    <h1 class="judul">Tentang Kami</h1>

    <div class="cerita">
      <div class="certext">
        <h2 class="txt">Cerita Kami</h2>

        <p>
          OnlineShop ini dikelola langsung oleh Siswa Yadika Soreang
          yang mantap dan hebat hahayyy.
        </p>
      </div>

      <div class="cerfot">
        <img :src="fotoCerita" alt="Foto Kami">
      </div>
    </div>

    <div class="crt">
      <h2 class="tim">Tim Kami</h2>

      <div class="teamlist">
        <TeamCard
          v-for="anggota in daftarTim"
          :key="anggota.nama"
          :nama="anggota.nama"
          :jabatan="anggota.jabatan"
        />
      </div>
    </div>
  </main>
</template>

<style scoped>
.content {
  text-align: center;
  font-size: 18px;
  margin-top: 20px;
  margin-right: 800px;
}

p {
  color: rgba(0, 0, 0, 0.514);
}

.abot {
  text-align: center;
  padding: 20px;
  background: linear-gradient(to right, #011d38, #000438);
  border-radius: 5px;
  margin-left: 20px;
  margin-right: 20px;
  color: white;
  margin-top: 13px;
}

.teamlist {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-top: 20px;
}

.tim {
  text-align: center;
  font-weight: 700;
  text-shadow: 2px 2px 5px rgba(2, 0, 0, 0.486);
}

.crt {
  display: flex;
  justify-content: center;
  text-align: center;
  flex-direction: column;
}


.cerita {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 20px 50px;
  gap: 30px;
}

.certext {
  flex: 1;
}

.cerfot {
  flex: 1;
  text-align: center;
}

.cerfot img {
  width: 350px;
  height: 230px;
  object-fit: cover;
  border-radius: 15px;
}
</style>

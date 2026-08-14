<script setup>
defineProps({
  nama: {
    type: String,
    required: true
  },
  jabatan: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="teamcard">
    <div class="avatar">
      {{ nama.charAt(0).toUpperCase() }}
    </div>

    <div class="info">
      <h3>{{ nama }}</h3>
      <p>{{ jabatan }}</p>
    </div>
  </div>
</template>

<style scoped>
.teamcard {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 20px;
  background-color: #ffffff;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
}

.avatar {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #4f46e5;
  color: white;
  font-size: 24px;
  font-weight: bold;
}

.info h3 {
  margin: 0 0 5px;
}

.info p {
  margin: 0;
  color: #666;
}
</style>

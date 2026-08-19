<template>
  <main>
    <h1 class="judul">Contact Us</h1>

    <div class="info">


      <div class="contact-info">
        <h2 class="txt">Contact Information</h2>
        <p>Alamat: RingRoad Alias jalan cingcin</p>
        <p>Email: Genjot@gmail.com</p>
        <p>Phone: 6666666666</p>
      </div>

      <div class="form">
        <form>
          <h2 class="txt">Hubungi</h2>

          <label>Name:</label>
          <input type="text">

          <label>Email:</label>
          <input type="email">

          <label>Message:</label>
          <textarea rows="4"></textarea>

          <button type="submit">Submit</button>
        </form>
      </div>

    </div>
  </main>
</template>

<style scoped>
.info {
  display: flex;
  gap: 20px;
  padding: 20px;
}

.form,
.contact-info {
  flex: 1;
  padding: 20px;
  border-radius: 10px;
  background: #f9f9f9;
}

input,
textarea {
  width: 100%;
  padding: 10px;
  margin: 5px 0 15px;
  border: 1px solid #ccc;
  border-radius: 5px;
  box-sizing: border-box;
}

.button1 {
   background: linear-gradient(to right, #010d18, #4A90E2);
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 999px;
}
</style>

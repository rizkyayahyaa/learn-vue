<template>
  <div id="app">
    <header>
      <h1>Selamat Datang di Proyek Vue.js</h1>
    </header>
    <div class="container">
      <aside class="sidebar">
        <h2>Menu</h2>
        <ul>
          
          <li><a href="#">Beranda</a></li>
          <li><a href="#">Tentang Kami</a></li>
          <li><a href="#">Layanan</a></li>
          <li><a href="#">Kontak</a></li>
        </ul>
      </aside>
      <main>
        <section class="hero">
          <h2>Halo, {{ name }}</h2>
          <p>Selamat datang di proyek Vue.js saya. Mari kita lihat bagaimana Vue.js dapat membantu Anda membuat aplikasi yang menakjubkan!</p>
          <button @click="changeName">Ubah Nama</button>
        </section>
      </main>
    </div>
    <footer>
      <p>&copy; 2024 Hak Cipta Dilarang</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "rizkya",
    };
  },
  methods: {
    changeName() {
      this.name = "yahya";
    }
  }
};
</script>

<style>
#app {
  font-family: 'Arial', sans-serif;
  text-align: center;
}

header {
  background-color: #4CAF50;
  color: white;
  padding: 20px;
}

.container {
  display: flex;
}

.sidebar {
  background-color: #333;
  color: white;
  width: 250px;
  padding: 20px;
}

.sidebar h2 {
  margin-bottom: 20px;
}

.sidebar ul {
  list-style-type: none;
  padding: 0;
}

.sidebar ul li {
  margin-bottom: 10px;
}

.sidebar ul li a {
  color: white;
  text-decoration: none;
}

.main {
  flex: 1;
  padding: 20px;
  background-color: #f2f2f2; /* tambahkan warna latar belakang */
}

button {
  background-color: #4CAF50;
  color: white;
  border: none;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin-top: 20px;
  cursor: pointer;
}

button:hover {
  background-color: #45a049;
}

footer {
  background-color: #333;
  color: white;
  padding: 20px;
}
</style>

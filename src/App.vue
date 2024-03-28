<template>
  <div id="app">
    <header>
      <h1>Selamat Datang di Proyek Vue.js</h1>
    </header>
    <main>
      <section class="hero">
        <div class="container">
          <h2>Halo, {{ name }}</h2>
          <p>Selamat datang di proyek Vue.js saya. Mari kita lihat bagaimana Vue.js dapat membantu Anda membuat aplikasi yang menakjubkan!</p>
          <button @click="changeName">Ubah Nama</button>
        </div>
      </section>
    </main>
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

.hero {
  background-color: #f2f2f2;
  padding: 50px 0;
}

.container {
  max-width: 800px;
  margin: auto;
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

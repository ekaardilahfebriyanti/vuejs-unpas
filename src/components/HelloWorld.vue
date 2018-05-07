<template>
  <div class="hello">

    <input type="text" v-model="namaDepan">
    <p>Nama Saya {{namaDepan}} <span v-html="namaBelakang"/></p>
    <p>Umur Saya {{umur}} tahun</p>
    <p>Status Saya {{status? 'jomblo':'single'}}</p>
    <p>Saya 
      <span v-show= "umur < 10"> Masih unyu unyu </span>
    </p>
    <a :href="akunFb" :title="umur < 10 ? 'muda' : 'tua'">Facebook</a>
    <ul>
      <li v-for="keluarga in daftarKeluarga">
        Daftar Keluarga {{keluarga.nama}} umur {{keluarga.umur+3}}
      </li>
    <button @mouseover="sapa('selamat datang')">Klik disini</button>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      namaDepan: "Hazar",
      namaBelakang: "<b>Tampan</b>",
      umur: 19,
      status: false,
      akunFb: "https://www.facebook.com/Ooneng23",
      daftarKeluarga: [
        { nama: "Bu iroh", umur: 33 },
        { nama: "Pak iroh", umur: 34 },
        { nama: "Nenek iroh", umur: 100 }
      ]
    };
  },
  methods: {
    sapa: function(text) {
      alert("hallo " + text);
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

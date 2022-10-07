<template>
  <h1>Biodata Diri</h1>
  <p>Nama: {{ nama }}</p>
  <p>Tempat, Tanggal Lahir : {{ ttl }}</p>
  <p>Alamat : {{ alamat }}</p>
  <p>Jenis Kelamin: {{ jk }}</p>
  <p>Status : {{ status }}</p>
  <p>Pekerjaan : {{ pekerjaan }}</p>
  <p>Agama : {{ agama }}</p>
</template>
<script>
  export default {
    name: "App",
    data() {
      return {
        nama: "Raja Indra Ramoza",
        ttl : "Pekanbaru, 18 Juni 2001",
        alamat: "Jl. Manyar Sakti, Tampan, Pekanbaru",
        jk :"Laki-laki",
        status:"Belum Menikah",
        pekerjaan : "Mahasiswa",
        agama :"Islam"
      };
    },
  };
  </script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1c2c7c;
  margin-top: 60px;
}
</style>

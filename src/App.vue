<script>
      export default{

        data(){
        return{
          dataMahasiswa:[],
          nama: "",
          nim: ""
        }
      },
        methods:{
          simpanData(){
            var mahasiswa={
              nama:this.nama,
              nim: this.nim
            }
            this.dataMahasiswa.push(mahasiswa);
        }
      }
      }
</script>

<template>
<div class="container">
  <form>
    <p class="alert alert-danger">Hello VueJs</p>
    <p>Nama</p>
    <input v-model="nama" type="text" class="form-text">
    <p>Nim</p>
    <input type="text" class="form-text">
    <div class="mt-2">
    <button class="btn btn-info" type="submit" @click.prevent="simpanData">Simpan</button>
    </div>
  </form>
</div>

<table class="table">
  <thead>
    <tr>
      <th>Nama</th>
      <th>Nim</th>
    </tr>
  </thead>
  <tbody>
    <tr :key="item.nama"  v-for="item in dataMahasiswa">
      <td>{{ item.nama }}</td>
      <td>{{ item.nim }}</td>
    </tr>
  </tbody>

</table>


</template>


<style>

</style>

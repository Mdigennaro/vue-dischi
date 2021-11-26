<template>
  <main>
    <div class="container">

      <Album 
      v-for="album in listaAlbum" 
      :key="album.id"
      :album="album"
      />

    </div>
  </main>
</template>

<script>
import axios from 'axios';
import Album from './Album.vue';

export default {
  nome: "Main",
  components:{
    Album,
  },
  data(){
    return{
      listaAlbum:[]
    }
  },
  methods:{
    getApi(){
      axios.get('https://flynn.boolean.careers/exercises/api/array/music')
      .then(r => {
        console.log('r',r);
        this.listaAlbum = r.data.response;
      })
      .catch(e =>{
        console.log(e);
      })
    }
  },
  mounted(){
    this.getApi();
  }
}
</script>

<style lang="scss">
@import '~@fontsource/be-vietnam-pro/index.css';


  main{
    height: calc(100% - 60px) ;
    background-color: #1e2d3b;
    padding-top: 40px;

    .container{
      width: 60%;
      min-width: 800px;
      height: 70vh;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
    }
  }

</style>
<template>
  <main>

    <div v-if="loaded" class="container">
      <Album 
      v-for="album in filteredAlbum" 
      :key="album.id"
      :album="album"
      />
    </div>

    <Loader class="caricamento" v-else/>

  </main>
</template>

<script>
import axios from 'axios';
import Album from './Album.vue';
import Loader from './Loader.vue';

export default {
  nome: "Main",
  components:{
    Album,
    Loader,
  },
  props:{
    genereAttivo: String
  },
  data(){
    return{
      listaAlbum:[],
      loaded: false,
      apiUrl: 'https://flynn.boolean.careers/exercises/api/array/music',
      genereSelezionato:'',
    }
  },
  computed:{
    filteredAlbum(){
      if (this.genereAttivo === ''){
        return this.listaAlbum;
      }
      
      return this.listaAlbum.filter(album =>{
        return album.genre === this.genereAttivo;
      })
    }
  },
  methods:{
    getApi(){
      axios.get(this.apiUrl)
      .then(r => {
        this.listaAlbum = r.data.response;
        this.loaded = true;
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
    padding-top: 20px;

    .container{
      width: 60%;
      min-width: 800px;
      height: 70vh;
      margin: 0 auto;
      display: flex;
      justify-content: flex-start;
      flex-wrap: wrap;

    }

    .caricamento{
      text-align: center;
      margin-top: 150px;
    }

  }

</style>
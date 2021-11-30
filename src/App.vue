<template>

  <div id="app">
    <Header @changeGenere="genereSelezionato" />
    <Main :genereAttivo="genereAttivo"/>
  </div>

</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
  },

  data(){
    return{
      genereAttivo:'',
    }
  },

  methods:{
    genereSelezionato(genre){

      this.genereAttivo = genre;
      console.log(genre);

    }
  }
}
</script>

<style lang="scss">
@import '~@fontsource/be-vietnam-pro/index.css';

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app{
  font-family: 'Be Vietnam Pro';
  height: 100vh;
  width: 100%;
  min-width: 900px;
}

</style>

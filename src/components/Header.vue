<template>
  <header class="logo">

    <img src="../assets/img/logo-spotify.png" alt="">

    <Selezione @sendSearch="genereSelezionato" />

  </header>
</template>

<script>
import Selezione from './Selezione.vue'

export default {
  nome: "Header",

  components:{
    Selezione
  },

  methods:{
    genereSelezionato(value){
      console.log('value', value);
    }
  }
}
</script>

<style lang="scss">

  .logo{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 60px;
    background-color: #2e3a46;

    img{
      width: 70px;
    }

  }

</style>
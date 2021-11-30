<template>
  <header class="logo">

    <img src="../assets/img/logo-spotify.png" alt="">

    <select name="genere" 
    id="genere"
    v-model="genre"
    @change="$emit('changeGenere',genre)"
    >
      <option value="" selected>Tutti i generi</option>
      <option value="Metal">Metal</option>
      <option value="Jazz">Jazz</option>
      <option value="Pop">Pop</option>
      <option value="Rock">Rock</option>
    </select>


  </header>
</template>

<script>

export default {
  nome: "Header",

  data(){
    return{
      genre :'',
    }
  },

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

    
    #genere{
      margin-right: 25px;
      background-color: #50d850;
      color: black;
      border: none;
      border-radius: 5px;
      padding: 10px 5px;
    }

  }

</style>
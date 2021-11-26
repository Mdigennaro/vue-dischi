<template>
  <div class="box-album">

    <img :src="album.poster" alt="">
    <h4>{{album.title}}</h4>
    <p>{{album.author}}</p>
    <p>{{album.year}}</p>

  </div>
</template>

<script>
export default {
  nome: "Album",
  props:{
    album: Object
  }
}
</script>

<style lang="scss">
@import '~@fontsource/be-vietnam-pro/index.css';

.box-album{
  flex-basis: calc(100% / 5 - 20px);
  height: 290px;
  background-color: #2e3a46;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
  margin-bottom: 20px;
  text-align: center;

  img{
    width: 100%;
  }

  h4{
    margin: 15px 0;
    color: white;
    text-transform: uppercase;
  }

  p{
    color: gray;
    font-size: 14px;
  }

  p:last-of-type{
    color: gray;
    font-size: 12px;
  }

}



</style>
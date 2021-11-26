<template>
  <div class="box-album">

    <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
    <h3>New Jersey</h3>
    <p>Bon Jovi</p>
    <p>1988</p>

  </div>
</template>

<script>
export default {
  nome: "AlbumList"
}
</script>

<style lang="scss">
@import '~@fontsource/be-vietnam-pro/index.css';




  .box-album{
    flex-basis: calc(100% / 5 - 20px);
    height: 280px;
    background-color: #2e3a46;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 20px;
    margin-bottom: 20px;

    img{
      width: 80%;
    }

    h3{
      margin: 10px 0;
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
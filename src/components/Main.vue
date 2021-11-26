<template>
  <main>
    <div class="container">

      <AlbumList />
      <AlbumList />
      <AlbumList />
      <AlbumList />
      <AlbumList />
      <AlbumList />
      <AlbumList />
      <AlbumList />
      <AlbumList />
      <AlbumList />

    </div>
  </main>
</template>

<script>
import AlbumList from './Albumlist.vue'

export default {
  nome: "Main",
  components:{
    AlbumList
  }
}
</script>

<style lang="scss">

  main{
    height: calc(100% - 60px) ;
    background-color: #1e2d3b;
    padding-top: 60px;

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
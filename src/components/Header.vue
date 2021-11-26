<template>
  <header class="logo">
    <img src="../assets/img/logo-spotify.png" alt="">
  </header>
</template>

<script>
export default {
  nome: "Header"
}
</script>

<style lang="scss">

  .logo{
    display: flex;
    align-items: center;
    width: 100%;
    height: 60px;
    background-color: #2e3a46;

    img{
      width: 70px;
    }
  }

</style>
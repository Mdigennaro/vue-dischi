<template>
  <div class="logo d-flex align-items-center">
    <img src="../assets/img/logo-spotify.png" alt="">
  </div>
</template>

<script>
export default {
  nome: "Header"
}
</script>

<style lang="scss">
@import '~bootstrap/scss/bootstrap.scss';

  .logo{
    width: 100%;
    height: 60px;
    background-color: #2e3a46;

    img{
      width: 70px;
    }
  }

</style>
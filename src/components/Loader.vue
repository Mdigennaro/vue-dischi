<template>

  <div>
    <h1>CARICAMENTO DEGLI ALBUM SPOTIFY...</h1>
    
  <div class="loadingio-spinner-double-ring-rzewyvhk3e"><div class="ldio-vyqtbnshsap">
<div></div>
<div></div>
<div><div></div></div>
<div><div></div></div>
</div></div>
  </div>
  
</template>

<script>
export default {
  name: "Loader"
}
</script>

<style lang="scss">

  h1{
    background-color: #50d850;
    margin:0 auto;
    width: 700px;
    color: black;
  }

  @keyframes ldio-vyqtbnshsap {
    0% { transform: rotate(0) }
    100% { transform: rotate(360deg) }
  }
  .ldio-vyqtbnshsap div { box-sizing: border-box!important }
  .ldio-vyqtbnshsap > div {
    position: absolute;
    width: 144px;
    height: 144px;
    top: 28px;
    left: 28px;
    border-radius: 50%;
    border: 16px solid #000;
    border-color: #50d850 transparent #50d850 transparent;
    animation: ldio-vyqtbnshsap 1s linear infinite;
  }

  .ldio-vyqtbnshsap > div:nth-child(2), .ldio-vyqtbnshsap > div:nth-child(4) {
    width: 108px;
    height: 108px;
    top: 46px;
    left: 46px;
    animation: ldio-vyqtbnshsap 1s linear infinite reverse;
  }
  .ldio-vyqtbnshsap > div:nth-child(2) {
    border-color: transparent #000000 transparent #000000
  }
  .ldio-vyqtbnshsap > div:nth-child(3) { border-color: transparent }
  .ldio-vyqtbnshsap > div:nth-child(3) div {
    position: absolute;
    width: 100%;
    height: 100%;
    transform: rotate(45deg);
  }
  .ldio-vyqtbnshsap > div:nth-child(3) div:before, .ldio-vyqtbnshsap > div:nth-child(3) div:after { 
    content: "";
    display: block;
    position: absolute;
    width: 16px;
    height: 16px;
    top: -16px;
    left: 48px;
    background: #50d850;
    border-radius: 50%;
    box-shadow: 0 128px 0 0 #50d850;
  }
  .ldio-vyqtbnshsap > div:nth-child(3) div:after {
    left: -16px;
    top: 48px;
    box-shadow: 128px 0 0 0 #50d850;
  }

  .ldio-vyqtbnshsap > div:nth-child(4) { border-color: transparent; }
  .ldio-vyqtbnshsap > div:nth-child(4) div {
    position: absolute;
    width: 100%;
    height: 100%;
    transform: rotate(45deg);
  }
  .ldio-vyqtbnshsap > div:nth-child(4) div:before, .ldio-vyqtbnshsap > div:nth-child(4) div:after {
    content: "";
    display: block;
    position: absolute;
    width: 16px;
    height: 16px;
    top: -16px;
    left: 30px;
    background: #000000;
    border-radius: 50%;
    box-shadow: 0 92px 0 0 #000000;
  }
  .ldio-vyqtbnshsap > div:nth-child(4) div:after {
    left: -16px;
    top: 30px;
    box-shadow: 92px 0 0 0 #000000;
  }
  .loadingio-spinner-double-ring-rzewyvhk3e {
    width: 200px;
    height: 200px;
    display: inline-block;
    overflow: hidden;
  }
  .ldio-vyqtbnshsap {
    width: 100%;
    height: 100%;
    position: relative;
    transform: translateZ(0) scale(1);
    backface-visibility: hidden;
    transform-origin: 0 0; /* see note above */
  }
  .ldio-vyqtbnshsap div { box-sizing: content-box; }

</style>


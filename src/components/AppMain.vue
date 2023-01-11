<script>
  export default {
    name: 'AppMain'
}

</script>

<template lang="">
  <div class="container">
    <div class="content-container" >
      <div class="col-2" >
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      </div>
      <div class="col-2" >
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
      </div>
      <div class="col-2" >
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
      </div>
      <div class="col-2" >
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
      </div>
      <div class="col-2" >
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
      </div>
    </div>
  </div>
</template>

<style lang="scss">
  .container{
    width: 100%;
    background-color: rgb(107, 107, 255);
    height: 200px;
  }
  .content-container{
    width: 70%;
    background-color: grey;
    height: 100%;
    display: flex;
  }
  .col-2{
    width: calc(100% / 5);
    background-color: orange;
    height: 100%;
    display: flex;
    align-items: center;
  }
</style>
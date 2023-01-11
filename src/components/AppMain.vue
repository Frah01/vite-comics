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
        <h3>DIGITAL COMICS</h3>
      </div>
      <div class="col-2" >
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        <h3>MERCHANDISE</h3>
      </div>
      <div class="col-2" >
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        <h3>SUBSCRIPTION</h3>
      </div>
      <div class="col-2" >
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        <h3>COMIC SHOP LOCATOR</h3>
      </div>
      <div class="col-2" >
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        <h3>DC POWER VISA</h3>
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
    height: 100%;
    display: flex;
  }
  .col-2{
    width: calc(100% / 5);
    display: flex;
    align-items: center;
  }

  .content-container img{
    width: 50px;
  }
  .content-container h3{
    color: white;
  }
</style>
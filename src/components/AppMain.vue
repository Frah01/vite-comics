<script>
  export default {
    name: 'AppMain',
    data(){
      return{
        images:[
          {
            image:"buy-comics-digital-comics.png",
            label: 'DIGITAL COMICS',
          },
          {
            image:"buy-comics-merchandise.png",
            label: 'MERCHANDISE',
          },
          {
            image:"buy-comics-subscriptions.png",
            label: 'SUBSCRIPTION',
          },
          {
            image:"buy-comics-shop-locator.png",
            label:  'COMIC SHOP LOCATOR',
          },
          {
            image:"buy-dc-power-visa.svg",
            label: 'DC POWER VISA',
          },
        ]
      }
    }
}

</script>
<template lang="">
  <div class="container">
    <div class="content-container" >
      <div class="col-2" v-for="(item,index) in images" :key="index" >
        <img :src="`/src/assets/img/${item.image}`">
        <h3>{{item.label}}</h3>
      </div>
     
    </div>
  </div>
</template>
<style lang="scss">
  .container{
    width: 100%;
    background-color: rgba(2,130,249,255);
    height: 200px;
    display: flex;
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
    h3{
      font-size: 13px;
    }
  }
  .content-container img{
    width: 50px;
  }
  .content-container h3{
    color: white;
  }

  
</style>
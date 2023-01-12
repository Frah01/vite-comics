<script>
export default {
    name: 'AppHeader',
    data(){
      return{
        list:[
          {
            item: 'CHARACTERS',
            state: false
          },
          {
            item: 'COMICS',
            state: false
          },
          {
            item: 'MOVIES',
            state: false
          },
          {
            item: 'TV',
            state: false
          },
          {
            item: 'GAMES',
            state: false
          },
          {
            item: 'COLLECTIBLES',
            state: false
          },
          {
            item: 'VIDEOS',
            state: false
          },
          {
            item: 'FANS',
            state: false
          },
          {
            item: 'NEWS',
            state: false
          },
          {
            item: 'SHOP',
            state: false
          },
        ]
      }
    }
}
</script>
<template lang="">
  <header>
    <div class="header-container">
      <div class="logo" >
       <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="navbar" >
        <ul class="list-header">
          <li v-for="(items, index) in list" :key="index">
            {{items.item}}
          </li>
        </ul>
      </div>
    </div>
  </header>
  <div class="container-second-header-section" >
    <div class="second-header-section" >
    <h1>content goes here</h1>
  </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as*;
@use '../styles/generals' as*;
  header{
    height: 150px;

  }
  .header-container{
    width: 70%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 100%;
  }
  .logo, .navbar{
    margin: 0;
  }
  .container-second-header-section{
  width: 100%;
  background-color: black;
}
  .second-header-section{
    width: 70%;
    height: 180px;
 
    color: white;
  }
.list-header{
  @include my-list-header
}
.list-header li{
 padding: 0px 5px;

 &.active{
  border-bottom: 3px solid blue
 }
}

.active-bar{
    height: 10px;
    width: 30px;
    background-color: blue;
  }
</style>
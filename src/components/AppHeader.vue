<script>
export default {
    name: 'AppHeader'
}
</script>

<template lang="">
  <header>
    <div class="header-container">
      <div class="logo" >
       <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="navbar" >
        <ul>
          <li>
            ciao
          </li>
        </ul>
      </div>
    </div>
  </header>
  <div class="second-header-section" >
    <h1>content goes here</h1>
  </div>
</template>

<style lang="scss">
@use '../styles/partials/mixins' as*;
@use '../styles/generals' as*;
  header{
    height: 150px;
    background-color: red;
  }

  .header-container{
    width: 70%;
    background-color: green;
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 100%;
  }
  .logo, .navbar{
    margin: 0;
  }

  .second-header-section{
    height: 80px;
    background-color: black;
    color: white;
  }


</style>
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
    justify-content: space-around;
    height: 100%;
  }
  .logo, .navbar{
    margin: 0;
  }

  .second-header-section{
    height: 180px;
    background-color: black;
    color: white;
  }


</style>
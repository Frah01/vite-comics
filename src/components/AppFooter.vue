<script>
export default {
    name: 'AppFooter'
}
</script>

<template lang="">
  <footer>
    <div class="footer-container" >
        <div class="col-50" >
          <ul class="list">
            <li>
              <h2>DC COMICS</h2>
            </li>
            <li>
              Characters
            </li>
            <li>
              Comics
            </li>
            <li>
              Movies
            </li>
            <li>
              TV
            </li>
            <li>
              Games
            </li>
            <li>
              Videos
            </li>
            <li>
              News
            </li>
          </ul>
          <ul class="list">
            <li>
              <h2>DC</h2>
            </li>
            <li>
              Characters
            </li>
            <li>
              Comics
            </li>
            <li>
              Movies
            </li>
            <li>
              TV
            </li>
            <li>
              Games
            </li>
            <li>
              Videos
            </li>
            <li>
              News
            </li>
          </ul>
          <ul class="list">
            <li>
              <h2>SITES</h2>
            </li>
            <li>
              Characters
            </li>
            <li>
              Comics
            </li>
            <li>
              Movies
            </li>
            <li>
              TV
            </li>
            <li>
              Games
            </li>
            <li>
              Videos
            </li>
            <li>
              News
            </li>
          </ul>
        </div>
        <div class="col-50">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </div>
  </footer>
  <div class="second-section-footer" >
    <div class="col-50" >
      <div class="" >
        <button class="button">SING-UP NOW!</button>
      </div>
    </div>
    <div class="col-50" >
      <div class="content-second-section-footer">
        <h3>FOLLOW US</h3>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@use '../styles/partials/mixins' as*;
  footer{
    width: 100%;
    background-color: rgb(22, 22, 22);
    height: 300px;
  }
  .footer-container{
    width: 70%;
    height: 100%;
    display: flex;
  }
  .col-50{
    width: 50%;
    height: 100%;
    display: flex;
    align-items: center;
  }

  .list{
    @include my-list;
  }

  footer li {
    padding: 5px;
  }
  
  footer img{
    width: 75%;
  }

  .second-section-footer{
    display: flex;
    width: 100%;
    height: 107px;
    background-color: black;
  }

  .button{
    @include my-button;
  }

  .content-second-section-footer{
    display: flex;
    h3{
      color: rgb(57, 57, 252);
    }
  }


  
</style>
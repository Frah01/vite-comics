<script>
export default {
    name: 'AppFooter',
    
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
            <li>
              <h2>SHOP</h2>
            </li>
            <li>
              Shop DC
            </li>
            <li>
              Shop DC Collectibles
            </li>
          </ul>
          <ul class="list">
            <li>
              <h2>DC</h2>
            </li>
            <li>
              Terms Of Use
            </li>
            <li>
              Privacy policy (New)
            </li>
            <li>
              Ad Choices
            </li>
            <li>
              Advertising
            </li>
            <li>
              Jobs
            </li>
            <li>
              Subscriptions
            </li>
            <li>
              Talent Workshops
            </li>
            <li>
              CPSC Certificates
            </li>
            <li>
              Ratings
            </li>
            <li>
              Shop Help
            </li>
            <li>
              Contact Us
            </li>
          </ul>
          <ul class="list">
            <li>
              <h2>SITES</h2>
            </li>
            <li>
              DC
            </li>
            <li>
              MAD Magazine
            </li>
            <li>
              DC Kids
            </li>
            <li>
              DC Universe
            </li>
            <li>
              DC Power Visa
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
        <button class="button">SING-UP NOW!</button>
    </div>
    <div class="col-50" >
      <div class="content-second-section-footer">
        <h3>FOLLOW US</h3>
        <img src="../assets/img/footer-facebook.png" alt="">
        <img src="../assets/img/footer-periscope.png" alt="">
        <img src="../assets/img/footer-pinterest.png" alt="">
        <img src="../assets/img/footer-twitter.png" alt="">
        <img src="../assets/img/footer-youtube.png" alt="">
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@use '../styles/partials/mixins' as*;
  footer{
    width: 100%;
    background-image: url(../assets/img/footer-bg.jpg);
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
    align-items: flex-start;
    
  }

  .second-section-footer .col-50 {
    align-items: center;
  }

  .list{
    @include my-list;
    margin: 50px 0px;
  }

  footer li {
    padding: 5px;
  }
  
  footer img{

  }

  .second-section-footer{
    display: flex;
    justify-content: center;
    background-color: rgba(48,48,48,255);
    padding: 20px 0px;
  }

  .button{
    @include my-button;
  }

  .content-second-section-footer{
    display: flex;
    align-items: center;
    h3{
      color: rgba(5,123,215,255);
      margin: 0px 10px;
    }
    img{
      margin: 0px 10px;
    }
  }


  
</style>
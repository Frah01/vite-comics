<script>
export default {
    name: 'AppFooter',
    data(){
      return{
        socials: [
          {
            logo: 'footer-facebook.png'
          },
          {
            logo: 'footer-periscope.png'
          },
          {
            logo: 'footer-pinterest.png'
          },
          {
            logo: 'footer-twitter.png'
          },
          {
            logo: 'footer-youtube.png'
          },
        ]
      }
    }
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
        <div class="col-50-dx">
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
        <div v-for="(item,index) in socials" :key="index">
          <img :src="`/src/assets/img/${item.logo}`">
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@use '../styles/partials/mixins' as*;
  footer{
    width: 100%;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
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

  .col-50-dx{
    background-repeat: no-repeat;
    background-image: url(../assets/img/dc-logo-bg.png);
    width: 50%;
  
    
  }

  .second-section-footer .col-50 {
    align-items: center;
  }

  .list{
    @include my-list;
    margin: 50px 0px;
    h2{
      color: white
    }
  }

  footer li {
    padding: 5px;
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
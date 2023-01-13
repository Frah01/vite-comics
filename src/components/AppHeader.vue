<script>
import imgCard from '../components/cartaImmagine.vue';
export default {
  components: {
    imgCard,
  },
  name: 'AppHeader',
  data() {
    return {
      list: [
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
      ],
      cards: [
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ],

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
      <div class="row-second-header-section" >
        <div v-for="(item,index) in cards" :key="index" >
          <imgCard :image="item.thumb" :titolo="item.series"></imgCard>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as*;
@use '../styles/generals' as*;

header {
  height: 150px;

}

.header-container {
  width: 70%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 100%;
}

.logo,
.navbar {
  margin: 0;
}

.container-second-header-section {
  width: 100%;
  background-color: rgba(28, 28, 28, 255);
}

.second-header-section {
  width: 70%;


}

.row-second-header-section {
  display: flex;
  flex-wrap: wrap;
}

.list-header {
  @include my-list-header
}

.list-header li {
  padding: 0px 5px;

  &.active {
    border-bottom: 3px solid blue
  }
}

.active-bar {
  height: 10px;
  width: 30px;
  background-color: blue;
}
</style>
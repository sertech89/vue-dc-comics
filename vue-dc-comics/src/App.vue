<template>
  <div id="app">
    <div class="container">
      <header>
          <LogoComp/>
          <NavbarComp/>
      </header>
    </div>
      
      <main>
        <JumboComp/>
         <div class="container">
          <div class="current-series">
            <div class="series-title">Current series</div>
            <SerieComp
              v-for="(element, index) in cards"
              :key="index"
              :details="element"
            />
            <div class="load-more">Load more</div>
          </div>
        </div>
       
      </main>
      
        <BlueMenuComp>
        </BlueMenuComp>

      <footer>
        <UpperFooterComp></UpperFooterComp>
        <BottomFooterComp></BottomFooterComp>
      </footer>
    
  </div>
</template>

<script>
import LogoComp from './components/LogoComp.vue';
import NavbarComp from './components/NavbarComp.vue';
import BlueMenuComp from './components/BlueMenuComp.vue';
import UpperFooterComp from './components/UpperFooterComp.vue';
import BottomFooterComp from './components/BottomFooterComp.vue';
import JumboComp from './components/JumboComp.vue';
import SerieComp from './components/SerieComp.vue';

export default {
  name: 'App',
  components: {
    LogoComp,
    NavbarComp,
    BlueMenuComp,
    UpperFooterComp,
    BottomFooterComp,
    JumboComp,
    SerieComp,
  },
  data() {
    return {
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
      ]
    }
  }
}
</script>

<style>

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body {
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif
  }
  .container {
    width: 75%;
    margin: 0 auto;
  }
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 0;
    background-color: white;
    color: #1c1c1c;
    font-weight: bold;
    font-size: 14px;
  }
  main {
    color: white;
    background-color: #1c1c1c;
  }
  main p {
    font-size: 22px;
    font-weight: bold;
  }

  .current-series {
    display: flex;
    flex-wrap: wrap;
    gap: 30px 10px;
    position: relative;
    background-color: #1c1c1c;
    padding: 40px 0;
  }
  
  .series-title {
    background-color: #0282f9;
    color: white;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 20px;
    padding: 5px 10px;
    width: 250px;
    text-align: center;
    position: absolute;
    top: -20px;
  }
  .load-more {
    font-weight: bold;
    background-color: #0282f9;
    color: white;
    text-transform: uppercase;
    padding: 5px 40px;
    position: absolute;
    left: 50%;
    bottom: 10px;
    transform: translateX(-50%);
  }

</style>
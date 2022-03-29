<template>
  <div class="dc-main">
    <section class="dc-main-top">
        <div id="jumbotron"></div>
        <div class="container">
            <MainComponent v-for="(element, index) in cards" :key="index" :cardObject="element" />
        </div>
    </section>
    <section class="dc-main-bottom">
        <div class="container">
            <ul>
                <li v-for="(element, index) in mainNav" :key="index">
                    <a :href="element.url">
                        <img :src="require(`../assets/img/${element.image}`)" :alt="element.title">
                        <h5>{{element.title}}</h5>
                    </a>
                </li>
            </ul>
        </div>
    </section>
  </div>
</template>

<script>
import MainComponent from './main_component/MainComponent.vue'

export default {
  name: 'IndexMain',
  components: {
      MainComponent
  },
  data: function(){
      return {
          mainNav: [
            {
                url: '#',
                image: 'buy-comics-digital-comics.png',
                title: 'digital comics'
            },
            {
                url: '#',
                image: 'buy-comics-merchandise.png',
                title: 'dc merchandise'
            },
            {
                url: '#',
                image: 'buy-comics-subscriptions.png',
                title: 'subscription'
            },
            {
                url: '#',
                image: 'buy-comics-shop-locator.png',
                title: 'comic shop locator'
            },
            {
                url: '#',
                image: 'buy-dc-power-visa.svg',
                title: 'dc power visa'
            }
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
          ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');
@import "../assets/scss/variables.scss";

    section.dc-main-top{
        width: 100vw;
        background-color: #1C1C1C;

        div#jumbotron {
            background-image: url(../assets/img/jumbotron.jpg);
            background-size: cover;
            background-repeat: no-repeat;
            background-position: top;
            width: 100vw;
            height: 400px;
            margin-bottom: 2rem;
        }

        h1{
        color: $colorWhite;
        }
    }

    section.dc-main-bottom{
        width: 100vw;
        height: 120px;
        background-color: $brandPrimary;

        ul{
            width: 100%;
            display: flex;
            justify-content: space-evenly;

            a{
                display: flex;

                img{
                    width: 40px;
                    height: 50px;
                    padding: 0 1rem;
                }

                h5{
                    font-weight: 300;
                    font-size: .8rem;
                    text-transform: uppercase;
                    color: $colorWhite;
                }
            }
        } 
    }
</style>
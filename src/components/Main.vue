<template>
  <div class="dc-main">
    <section class="dc-main-top">
        <div class="container">
            <h1>--> Content goes here</h1>
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
export default {
  name: 'IndexMain',
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
          ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');
@import "../assets/scss/variables.scss";

    section.dc-main-top{
        width: 100vw;
        height: 15vh;
        background-color: #1C1C1C;

        h1{
        color: $colorWhite;
        }
    }

    section.dc-main-bottom{
        width: 100vw;
        height: 17vh;
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
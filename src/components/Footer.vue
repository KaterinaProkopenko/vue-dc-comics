<template>
  <div class="dc-footer">
      <section class="footer-top">
          <div class="container">
              <div class="footer-list">
                  <div>
                      <h4>dc comics</h4>
                      <ul>
                          <li v-for="(element, index) in comics" :key="index">
                              <a :href="element.url">{{element.text}}</a>
                          </li>
                      </ul>

                      <h4>shop</h4>
                      <ul>
                          <li v-for="(element, index) in shop" :key="index">
                              <a :href="element.url">{{element.text}}</a>
                          </li>
                      </ul>
                  </div>
                  <div class="footer-list-middle">
                      <h4>dc</h4>
                      <ul>
                          <li v-for="(element, index) in dc" :key="index">
                              <a :href="element.url">{{element.text}}</a>
                          </li>
                      </ul>
                  </div>
                  <div>
                      <h4>sites</h4>
                      <ul>
                          <li v-for="(element, index) in sites" :key="index">
                              <a :href="element.url">{{element.text}}</a>
                          </li>
                      </ul>
                  </div>
              </div>
              <div class="logo-bg"></div>
          </div>
      </section>
      <section class="footer-bottom">
          <div class="container">
              <a href="#">sign-up now!</a>
              <div class="social-media">
                  <h3>follow us</h3>
                  <img src="../assets/img/footer-facebook.png" alt="facebook">
                  <img src="../assets/img/footer-twitter.png" alt="twitter">
                  <img src="../assets/img/footer-youtube.png" alt="youtube">
                  <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                  <img src="../assets/img/footer-periscope.png" alt="periscope">
              </div>
          </div>
      </section>
  </div>
</template>

<script>
export default {
  name: 'IndexFooter',
  data: function() {
      return {
          comics: [
              {
                  url: '#',
                  text: 'Characters'
              },
              {
                  url: '#',
                  text: 'Comics'
              },
              {
                  url: '#',
                  text: 'Movies'
              },
              {
                  url: '#',
                  text: 'TV'
              },
              {
                  url: '#',
                  text: 'Games'
              },
              {
                  url: '#',
                  text: 'Videos'
              },
              {
                  url: '#',
                  text: 'News'
              }
          ],
          shop: [
              {
                  url: '#',
                  text: 'Shop DC'
              },
              {
                  url: '#',
                  text: 'Shop DC Collectibles'
              }
          ],
          dc: [
              {
                  url: '#',
                  text: 'Terms Of Use'
              },
              {
                  url: '#',
                  text: 'Privacy policy (New)'
              },
              {
                  url: '#',
                  text: 'Ad Choices'
              },
              {
                  url: '#',
                  text: 'Advertising'
              },
              {
                  url: '#',
                  text: 'Jobs'
              },
              {
                  url: '#',
                  text: 'Subscriptions'
              },
              {
                  url: '#',
                  text: 'Talent Workshops'
              },
              {
                  url: '#',
                  text: 'CPSC Certificates'
              },
              {
                  url: '#',
                  text: 'Ratings'
              },
              {
                  url: '#',
                  text: 'Shop Help'
              },
              {
                  url: '#',
                  text: 'Contact Us'
              }
          ],
          sites: [
              {
                  url: '#',
                  text: 'DC'
              },
              {
                  url: '#',
                  text: 'MAD Magazine'
              },
              {
                  url: '#',
                  text: 'DC Kids'
              },
              {
                  url: '#',
                  text: 'DC Universe'
              },
              {
                  url: '#',
                  text: 'DC Power Visa'
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

    div.dc-footer{
        width: 100vw;
        height: 53vh;

        section.footer-top{
            width: 100vw;
            min-width: 900px;
            height: 39vh;
            background-image: url(../assets/img/footer-bg.jpg);
            background-size: cover;
            background-repeat: no-repeat;
            background-position: center;

            div.footer-list{
                margin-top: 1.2rem;
                display: flex;
            }

            div.footer-list-middle{
                margin: 0 1.5rem;
            }

            div.logo-bg{
                width: 450px;
                height: 100%;
                background-image: url(../assets/img/dc-logo-bg.png);
                background-size: 100%;
                background-position-y: center;
            }

            a{
                color: gray;
                font-size: .7rem;
            }
        }

        section.footer-bottom{
            width: 100%;
            height: 14vh;
            background-color: #303030;
            text-transform: uppercase;

            a{
                color: $colorWhite;
                border: 2px solid $brandPrimary;
                padding: .6rem;
            }

            

            div.social-media{
                display: flex;
                align-items: center;

                h3{
                    color: $brandPrimary;
                    padding-right: .5rem;
                }
                
                img{
                    width: 30px;
                    height: 30px;
                    margin-left: 1rem;
                }
            }
        }
    }

    h4{
        text-transform: uppercase;
        color: $colorWhite;
        margin: 0;
        padding: .7rem 0;
    }

    ul{
        padding-left: 0;
        padding-bottom: .3rem;
        margin: 0;

        li{
            line-height: .9rem;
        }
    }

</style>
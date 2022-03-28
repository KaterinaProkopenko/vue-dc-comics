<template>
  <div class="dc-footer">
      <section class="footer-top">
          <div class="container">
              <div class="footer-list">
                  <div>
                      <h4>dc comics</h4>
                      <ul>
                          <li>
                              <a href="#">Characters</a>
                          </li>
                          <li>
                              <a href="#">Comics</a>
                          </li>
                          <li>
                              <a href="#">Movies</a>
                          </li>
                          <li>
                              <a href="#">TV</a>
                          </li>
                          <li>
                              <a href="#">Games</a>
                          </li>
                          <li>
                              <a href="#">Videos</a>
                          </li>
                          <li>
                              <a href="#">News</a>
                          </li>
                      </ul>

                      <h4>shop</h4>
                      <ul>
                          <li>
                              <a href="#">Shop DC</a>
                          </li>
                          <li>
                              <a href="#">Shop DC Collectibles</a>
                          </li>
                      </ul>
                  </div>
                  <div class="footer-list-middle">
                      <h4>dc</h4>
                      <ul>
                          <li>
                              <a href="#">Terms Of Use</a>
                          </li>
                          <li>
                              <a href="#">Privacy policy (New)</a>
                          </li>
                          <li>
                              <a href="#">Ad Choices</a>
                          </li>
                          <li>
                              <a href="#">Advertising</a>
                          </li>
                          <li>
                              <a href="#">Jobs</a>
                          </li>
                          <li>
                              <a href="#">Subscriptions</a>
                          </li>
                          <li>
                              <a href="#">Talent Workshops</a>
                          </li>
                          <li>
                              <a href="#">CPSC Certificates</a>
                          </li>
                          <li>
                              <a href="#">Ratings</a>
                          </li>
                          <li>
                              <a href="#">Shop Help</a>
                          </li>
                          <li>
                              <a href="#">Contact Us</a>
                          </li>
                      </ul>
                  </div>
                  <div>
                      <h4>sites</h4>
                      <ul>
                          <li>
                              <a href="#">DC</a>
                          </li>
                          <li>
                              <a href="#">MAD Magazine</a>
                          </li>
                          <li>
                              <a href="#">DC Kids</a>
                          </li>
                          <li>
                              <a href="#">DC Universe</a>
                          </li>
                          <li>
                              <a href="#">DC Power Visa</a>
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
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');

    div.dc-footer{
        width: 100vw;
        height: 53vh;
        font-family: Roboto Condensed;
    }

    section.footer-top{
        width: 100vw;
        min-width: 900px;
        height: 39vh;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
    }

    section.footer-bottom{
        width: 100%;
        height: 14vh;
        background-color: #303030;
        text-transform: uppercase;
    }

    div.container{
        width: 1000px;
        height: 100%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

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

    section.footer-top h4{
        text-transform: uppercase;
        color: white;
        margin: 0;
        padding: .7rem 0;
    }

    ul{
        padding-left: 0;
        padding-bottom: .3rem;
        margin: 0;
    }

    li{
        list-style-type: none;
        line-height: .9rem;
    }

    section.footer-top a{
        text-decoration: none;
        color: gray;
        font-size: .7rem;
    }

    section.footer-bottom a{
        text-decoration: none;
        color: white;
        border: 2px solid #0282F9;
        padding: .6rem;
    }

    section.footer-bottom h3{
        color: #0282F9;
        padding-right: .5rem;
    }

    div.social-media{
        display: flex;
        align-items: center;

    }

    div.social-media img{
        width: 30px;
        height: 30px;
        margin-left: 1rem;
    }
</style>
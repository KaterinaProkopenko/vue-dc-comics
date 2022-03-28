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
                <li>
                    <a href="#">
                        <img id="img-digital-comics" src="../assets/img/buy-comics-digital-comics.png" alt="Buy comics digital">
                        <h5>digital comics</h5>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img id="img-merchandise" src="../assets/img/buy-comics-merchandise.png" alt="Buy comics merchandise">
                        <h5>dc merchandise</h5>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img id="img-subscription" src="../assets/img/buy-comics-subscriptions.png" alt="Buy comics subscriptions">
                        <h5>subscription</h5>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img id="img-shop-locator" src="../assets/img/buy-comics-shop-locator.png" alt="Buy comics shop locator">
                        <h5>comic shop locator</h5>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img id="power-visa" src="../assets/img/buy-dc-power-visa.svg" alt="Buy dc power visa">
                        <h5>dc power visa</h5>
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
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');

    section.dc-main-top{
        width: 100vw;
        height: 15vh;
        background-color: #1C1C1C;
    }

    section.dc-main-bottom{
        width: 100vw;
        height: 17vh;
        background-color: #0282F9;
    }

    div.container{
        width: 1000px;
        height: 100%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    h1{
        color: white;
    }
    
    ul{
        width: 100%;
        display: flex;
        justify-content: space-evenly;
    }

    li{
        list-style-type: none;
    }

    a{
        text-decoration: none;
        display: flex;
    }

    img{
        padding: 0 1rem;
    }

    h5{
        font-weight: 300;
        font-size: .7rem;
        text-transform: uppercase;
        color: white;
    }

    img#img-digital-comics{
        width: 35px;
        height: 45px;
    }

    img#img-merchandise{
        width: 41px;
        height: 43px;
    }

    img#img-subscription{
        width: 45px;
        height: 45px;
    }

    img#img-shop-locator{
        width: 30px;
        height: 45px;
    }

    img#power-visa{
        width: 45px;
        height: 40px;
    }
</style>
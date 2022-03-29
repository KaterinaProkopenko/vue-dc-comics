<template>
  <div class="dc-header">
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="DC logo">
      <ul>
        <li v-for="(element, index) in headerNavList" :key="index" :class="(element.active) ? 'active' : ''">
          <a :class="(element.active) ? 'active-link' : ''" :href="element.url">{{element.text}}</a>
        </li>
      </ul>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'IndexHeader',
  data: function() {
    return {
      headerNavList: [
        {
          text: 'characters',
          url: '#',
          active: false
        },
        {
          text: 'comics',
          url: '#',
          active: true
        },
        {
          text: 'movies',
          url: '#',
          active: false
        },
        {
          text: 'tv',
          url: '#',
          active: false
        },
        {
          text: 'games',
          url: '#',
          active: false
        },
        {
          text: 'collectibles',
          url: '#',
          active: false
        },
        {
          text: 'videos',
          url: '#',
          active: false
        },
        {
          text: 'fans',
          url: '#',
          active: false
        },
        {
          text: 'news',
          url: '#',
          active: false
        },
        {
          text: 'shop',
          url: '#',
          active: false
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

  div.dc-header{
    width: 100vw;
    height: 110px;
    font-weight: 700;

    img{
      width: 65px;
      height: 65px; 
    }

    ul{
      display: flex;
      justify-content: space-between;
      width: 70%;
      height: 100%;
      margin: 0;

      li{
        display: flex;
        align-items: center;

        a{
          color: #2c2c2c;
          font-size: .8rem;
          text-transform: uppercase;
        }
      }
    }
  }
  .active{
    border-bottom: 4px solid $brandPrimary;
  }

  .active-link {
    color: $brandPrimary;
  }
</style>
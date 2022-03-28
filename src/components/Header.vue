<template>
  <div class="dc-header">
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="DC logo">
      <ul>
        <li>
          <a href="#">characters</a>
        </li>
        <li>
          <a class="active" href="#">comics</a>
        </li>
        <li>
          <a href="#">movies</a>
        </li>
        <li>
          <a href="#">tv</a>
        </li>
        <li>
          <a href="#">games</a>
        </li>
        <li>
          <a href="#">collectibles</a>
        </li>
        <li>
          <a href="#">videos</a>
        </li>
        <li>
          <a href="#">fans</a>
        </li>
        <li>
          <a href="#">news</a>
        </li>
        <li>
          <a href="#">shop</a>
        </li>
      </ul>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'IndexHeader',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');

  div.dc-header{
    width: 100vw;
    height: 15vh;
    font-family: Roboto Condensed;
    font-weight: 700;
  }

  div.container{
    width: 1000px;
    height: 100%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  img{
    width: 65px;
    height: 65px; 
  }

  ul{
    display: flex;
    justify-content: space-between;
    width: 70%;
    height: 15vh;
    margin: 0;
  }

  li{
    list-style-type: none;
    height: 100%;
    display: flex;
    align-items: center;
  }

  a{
    text-decoration: none;
    color: #384033;
    font-size: .9rem;
  }

  .active{
    color: #0282F9;
    border-bottom: 4px solid #0282F9;
  }
</style>
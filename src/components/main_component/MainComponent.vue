<template>
  <div class="card">
    <img :src="cardObject.thumb" :alt="cardObject.series">
    <h5>{{cardObject.series}}</h5>
      
  </div>
</template>

<script>
export default {
    name: 'IndexCard',
    props: ['cardObject']
}
</script>

<style lang="scss" scoped>
@import "../../assets/scss/variables.scss";

  div.card{
    flex-basis: calc(85% / 6);
    height: 250px;

    img{
      width: 100%;
      height: 170px;
    }

    h5{
      margin: 0;
      padding: .5rem;
      text-transform: uppercase;
      color: $colorWhite;
      font-weight: 300;
    }
  }

    
</style>
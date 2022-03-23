<template>
  <div class="card-holder">
    <div class="card">
        <img :src="img" :alt="imgAlt">

    </div>
    <h3>{{seriesText}}</h3>
  </div>


</template>

<script>
export default {
name: 'CurrentSeriesDC',
props: {
  img: String,
  seriesText: String,
  imgAlt: String
}
}
</script>

<style scoped lang="scss">
  @import "../assets/styles/main";
  .card-holder {
    width: calc(100% / 6 - 1rem);
    height: 100%;
    margin: 0 .5rem 2rem .5rem;
  }
  .card {
    height: 9.5rem;
    margin-bottom: .5rem;
    img {
      width: 100%;
      height: 100%;
      overflow: hidden;
      object-fit: cover;
      object-position: 50% 0%;
    }
  }
  h3 {
      margin-top: .3rem;
      text-transform: uppercase;
      font-size: 11px;
      color: white;
    }
</style>

<template>
  <div class="card-holder">
    <div class="card">
        <img :src="img" :alt="imgAlt">
        <h3>{{seriesText}}</h3>
    </div>
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
    margin: 0 .5rem 2rem .5rem;
    width: calc(100% / 6 - 1rem);
    height: 12rem;
  }

  .card {
    width: 100%;
    height: 100%;
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
      text-transform: uppercase;
      font-size: 11px;
      color: white;
    }
</style>

<template>

    <div class="card">
        <img :src="img" :alt="imgAlt">
        <h3>{{cardText}}</h3>
    </div>

</template>

<script>
export default {
name: 'CardsDC',
props: {
  img: String,
  cardText: String,
  imgAlt: String
}
}
</script>

<style scoped lang="scss">
  @import "../assets/styles/main";

  .card {
        display: flex;
        align-items: center;
        gap: 8px;
        text-transform: uppercase;
        h3 {
          font-size: 11px;
          color: white;
        }
        img {
          max-height: 3rem;
        }
  }
</style>

<template>
    <div class="card">
      <div class="card-image">
        <img :src="comic.thumb" :alt="comic.series">
      </div>
      <div class="card-text">{{ comic.series }}</div>
    </div>
</template>

<script>
export default {
  name: 'ComicCard',
  props: ['comic']
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";

  .card {
    width: calc(100% / 6 - 1.5625rem);
    margin-bottom: 3rem;
    cursor: pointer;

    .card-image {
      position: relative;
      display: block;
      margin-bottom: 20px;

      &::before{
        display: block;
        content: "";
        padding-top: 100%;
      }

      img {
        position: absolute;
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
        top: 0;
      }
    }

    &-text {
      font-size: 1.25rem;
      color: $lightColor;
      text-transform: uppercase;
    }
  }
</style>
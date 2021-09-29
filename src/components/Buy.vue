<template>
  <section>
    <div class="container">
      <div class="item">
        <div class="item-img">
          <img src="@/assets/images/buy-comics-digital-comics.png" alt="digital comics">
        </div>
        <div class="item-text">digital comics</div>
      </div>
      <div class="item">
        <div class="item-img">
          <img src="@/assets/images/buy-comics-digital-comics.png" alt="digital comics">
        </div>
        <div class="item-text">digital comics</div>
      </div>
      <div class="item">
        <div class="item-img">
          <img src="@/assets/images/buy-comics-digital-comics.png" alt="digital comics">
        </div>
        <div class="item-text">digital comics</div>
      </div>
      <div class="item">
        <div class="item-img">
          <img src="@/assets/images/buy-comics-digital-comics.png" alt="digital comics">
        </div>
        <div class="item-text">digital comics</div>
      </div>
      <div class="item">
        <div class="item-img">
          <img src="@/assets/images/buy-comics-digital-comics.png" alt="digital comics">
        </div>
        <div class="item-text">digital comics</div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Buy'
}
</script>

<style lang="scss" scoped>
  @import '@/assets/style/variables';

  section{
    background-color: $secondaryColor;
  }
  .container{
    display: flex;
    justify-content: space-around;
    padding: 3rem 0;

    .item{
      display: flex;
      align-items: center;

      &-img{
        height: 3.125rem;

        img{
          height: 100%;
        }
      }
      &-text{
        margin-left: 1rem;
        color: $lightColor;
        text-transform: uppercase;
      }
    }
  }

</style>
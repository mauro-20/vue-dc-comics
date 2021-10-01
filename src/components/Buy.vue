<template>
  <section>
    <div class="container">
      <div class="item" v-for="(item, index) in items" :key="index">
        <div class="item-img">
          <img :src="item.src" :alt="item.text">
        </div>
        <div class="item-text">{{item.text}}</div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Buy',
  data() {
    return {
      items: [
        {
          src: require('../assets/images/buy-comics-digital-comics.png'),
          text: 'digital comics'
        },
        {
          src: require('../assets/images/buy-comics-merchandise.png'),
          text: 'dc merchandise'
        },
        {
          src: require('../assets/images/buy-comics-subscriptions.png'),
          text: 'subscription'
        },
        {
          src: require('../assets/images/buy-comics-shop-locator.png'),
          text: 'comic shop locator'
        },
        {
          src: require('../assets/images/buy-dc-power-visa.svg'),
          text: 'dc power visa'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

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
      cursor: pointer;

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
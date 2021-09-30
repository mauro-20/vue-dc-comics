<template>
  <div class="footer-bottom">
    <div class="container">
      <div class="col-left">
        <a href="#">sign-up now!</a>
      </div>
      <div class="col-right">
        <div class="col-right-follow">follow us</div>
        <ul>
          <li v-for="(social, index) in socials" :key="index">
            <img :src="social.src">
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterBottom',
  data() {
    return {
      socials: [
        {
          src: require('../assets/images/footer-facebook.png'),
          url: '#'
        },
        {
          src: require('../assets/images/footer-twitter.png'),
          url: '#'
        },
        {
          src: require('../assets/images/footer-youtube.png'),
          url: '#'
        },
        {
          src: require('../assets/images/footer-pinterest.png'),
          url: '#'
        },
        {
          src: require('../assets/images/footer-periscope.png'),
          url: '#'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '@/assets/style/variables';
  
  .footer-bottom{
    background-color: $footerColor;
    padding: 3rem;
  }
  .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .col{

    &-left{
      a{
        padding: .875rem;
        border: .125rem solid $secondaryColor;
        background-color: $footerColor;
        color: $lightColor;
        text-transform: uppercase;
      }
    }
    &-right{
      display: flex;
      align-items: center;
      &-follow{
        font-weight: 900;
        font-size: 1.25rem;
        text-transform: uppercase;
        color: $secondaryColor;
      }
      ul{
        display: flex;
        li{
          margin-left: 1rem;
          cursor: pointer;
        }
      }
    }
  }

</style>
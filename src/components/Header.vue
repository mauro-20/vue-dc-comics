<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="../assets/images/dc-logo.png" alt="logo DC">
      </div>
      <nav>
        <ul>
          <li v-for="(link, index) in menu" :key="index">
            <a :href="link.url" :class="{current: link.current}">{{link.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
		return {
			menu: [
              {
                  text: "characters",
                  url: "#",
                  current: false,
              },
              {
                  text: "comics",
                  url: "#",
                  current: true,
              },
              {
                  text: "movies",
                  url: "#",
                  current: false,
              },
              {
                  text: "tv",
                  url: "#",
                  current: false,
              },
              {
                  text: "games",
                  url: "#",
                  current: false,
              },
              {
                  text: "collectibles",
                  url: "#",
                  current: false,
              },
              {
                  text: "videos",
                  url: "#",
                  current: false,
              },
              {
                  text: "fans",
                  url: "#",
                  current: false,
              },
              {
                  text: "news",
                  url: "#",
                  current: false,
              },
              {
                  text: "shop",
                  url: "#",
                  current: false,
              }
            ],
		}
	}
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables';

  header{
    background-color: $lightColor;
  }

  .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.25rem 0;

    .logo{
      height: 6rem;

      img{
        height: 100%;
      }
    }
    
    ul{
      display: flex;

      li{
        margin: 0 1.25rem;
      }
      a{
        text-transform: uppercase;
        font-weight: 700;
        color: $primaryColor;
        padding: 3.1875rem 0;
        border-bottom: .3125rem solid transparent;

        &.current{
          color: $secondaryColor;
          border-bottom: .3125rem solid $secondaryColor;
          
        }

      }
    }

  }


</style>
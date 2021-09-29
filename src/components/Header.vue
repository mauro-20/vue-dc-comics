<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="../assets/images/dc-logo.png" alt="logo DC">
      </div>
      <nav>
        <ul>
          <li>
            <a href="#">home</a>
          </li>
          <li>
            <a href="#" class="current">shop</a>
          </li>
          <li><a href="#">car</a></li>
          <li><a href="#">spiderman</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="scss" scoped>
@import '@/assets/style/variables';

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
      list-style: none;

      li{
        margin: 0 1.25rem;
      }
      a{
        text-decoration: none;
        text-transform: uppercase;
        font-weight: 700;
        color: $primaryColor;
        padding: 3.1875rem 0;
        border-bottom: .3125rem solid $lightColor;

        &.current{
          color: $secondaryColor;
          border-bottom: .3125rem solid $secondaryColor;
          
        }

      }
    }

  }


</style>
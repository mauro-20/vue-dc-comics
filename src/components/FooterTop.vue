<template>
  <div class="footer-top">
    <div class="container">
      <div class="col">
        <h3>dc comics</h3>
        <ul>
          <li><a href="#">characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
          <li><a href="#">tv</a></li>
          <li><a href="#">characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
          <li><a href="#">tv</a></li>
        </ul>
        <h3>dc comics</h3>
        <ul>
          <li><a href="#">characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
        </ul>
      </div>
      <div class="col">
        <h3>dc comics</h3>
        <ul>
          <li><a href="#">characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
          <li><a href="#">tv</a></li>
          <li><a href="#">characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
          <li><a href="#">tv</a></li>
          <li><a href="#">tv</a></li>
          <li><a href="#">characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
          <li><a href="#">tv</a></li>
        </ul>
      </div>
      <div class="col">
        <h3>dc comics</h3>
        <ul>
          <li><a href="#">characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
          <li><a href="#">tv</a></li>
          <li><a href="#">characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
          <li><a href="#">tv</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterTop'
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';
  
  .footer-top{
    background-image: url('../assets/images/footer-bg.jpg');
    background-size: cover;
  }
  .container{
    display: flex;
    padding: 2.5rem 0;
    background-image: url('../assets/images/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: right;
  }

  .col{
    margin-right: 2rem;

    h3{
      margin: 1.25rem 0;
      text-transform: uppercase;
      color: $lightColor;
    }
    a{
      text-transform: capitalize;
      color: #596564;
    }
  }

</style>
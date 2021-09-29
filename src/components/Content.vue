<template>
  <section>
    <div class="container">
    --> Content goes here --
    </div>
  </section>
</template>

<script>
export default {
  name: 'Content'
}
</script>

<style lang="scss" scoped>
  @import '@/assets/style/variables';
  
  section{
    color: $lightColor;
    font-size: 2rem;
    background-color: $primaryColor;
    padding: 3rem;
  }

</style>
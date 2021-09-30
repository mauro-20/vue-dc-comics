<template>
  <section>
    <img src="../assets/images/jumbotron.jpg" alt="jumbo">
  </section>
</template>

<script>
export default {
  name: 'Hero'
}
</script>

<style lang="scss" scoped>
  section{
    height: 20rem;
    overflow: hidden;

    img{
      width: 100%;
      object-fit: contain;
    }
  }

</style>
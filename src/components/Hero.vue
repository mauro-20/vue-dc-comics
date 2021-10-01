<template>
  <section>
    <img :src="src" alt="jumbo">
  </section>
</template>

<script>
export default {
  name: 'Hero',
  props: ['src']
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
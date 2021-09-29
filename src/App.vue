<template>
  <div id="app">
    <Header/>
    <main>
      <Content/>
      <Buy/>
    </main>
    <footer>
      <FooterTop/>

    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Buy from "./components/Buy.vue";
import Content from './components/Content.vue';
import FooterTop from "./components/FooterTop.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Buy,
    FooterTop
  },
};
</script>

<style lang="scss">
  @import "@/assets/style/common";

</style>

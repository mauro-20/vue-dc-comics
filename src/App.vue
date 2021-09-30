<template>
  <div id="app">
    <Header/>
    <main>
      <Hero/>
      <Comics/>
      <!-- <Content/> -->
      <Buy/>
    </main>
    <footer>
      <FooterTop/>
      <FooterBottom/>
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import Comics from "./components/Comics.vue";
// import Content from './components/Content.vue';
import Buy from "./components/Buy.vue";
import FooterTop from "./components/FooterTop.vue";
import FooterBottom from "./components/FooterBottom.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    Comics,
    // Content,
    Buy,
    FooterTop,
    FooterBottom
  },
};
</script>

<style lang="scss">
  @import "@/assets/style/common";

</style>

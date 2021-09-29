<template>
  <div id="app">
    <Header />
    <main>
      <Content/>
      <Buy/>
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Buy from "./components/Buy.vue";
import Content from './components/Content.vue';
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Buy,
    Footer
  },
};
</script>

<style lang="scss">
@import "@/assets/style/common";

body {
  background-color: #0ff;
}
</style>

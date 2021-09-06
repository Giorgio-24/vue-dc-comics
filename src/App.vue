<template>
  <div id="app">
    <Header />
    <main>
      <Content />
      <Shop />
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import Shop from "./components/Dc-shop.vue" ;

export default {
  name: "App",
  components: {
    Header,
    Content,
    Shop,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/style.scss";
</style>

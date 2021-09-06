<template>
  <div id="app">
    <Header />
    <main>
      <Content />
    </main>
    <footer>
      <div>
        <Shop />
        <FooterLinks />
      </div>
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import Shop from "./components/Dc-shop.vue";
import FooterLinks from "./components/Links-list.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Shop,
    FooterLinks,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/style.scss";
</style>

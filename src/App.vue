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
      <Footer />
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import Shop from "./components/Dc-shop.vue";
import FooterLinks from "./components/Links-list.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Shop,
    FooterLinks,
    Footer,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/style.scss";
</style>

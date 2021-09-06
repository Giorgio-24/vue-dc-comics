<template>
  <section>
    <div class="container h-100">
      <ul class="h-100">
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.href"
            ><img :src="link.icon" :alt="`buy-${link.text}`" /><span>{{
              link.text
            }}</span></a
          >
        </li>

        <!--         <li><a href="#">DC merchandise</a></li>
        <li><a href="#">Subscription</a></li>
        <li><a href="#">Comic shop locator</a></li>
        <li><a href="#">Dc power visa</a></li> -->
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "Data",
  data() {
    return {
      links: [
        {
          text: "digital comics",
          icon: "../src/assets/img/buy-comics-digital-comics.png",
          href: "#",
        },
        {
          text: "dc merchandise",
          icon: "../src/assets/img/buy-comics-merchandise.png",
          href: "#",
        },
        {
          text: "subscription",
          icon: "../src/assets/img/buy-comics-subscriptions.png",
          href: "#",
        },
        {
          text: "comic shop locator",
          icon: "../src/assets/img/buy-comics-shop-locator.png",
          href: "#",
        },
        {
          text: "dc power visa",
          icon: "../src/assets/img/buy-dc-power-visa.svg",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_vars.scss";
@import "@/assets/scss/_mixins.scss";

section {
  height: 150px;
  background-color: $blue;

  ul {
    @include center("y");
    @include justify("around");
    li {
      @include center("y");

      a {
        color: #fff;
        text-transform: uppercase;
        padding: 25px;
        &:hover {
          color: #000;
        }
      }
    }
  }
}
</style>
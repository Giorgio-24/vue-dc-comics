<template>
  <header class="container">
    <div class="row">
      <figure>
        <img src="@/assets/img/dc-logo.png" alt="dc-logo" class="img-fluid" />
      </figure>
      <ul>
        <li class="d-inline-block" v-for="(link, index) in links" :key="index">
          <a class="uppercase" :href="link.url">{{ link.text }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Data",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_mixins.scss";
@import "@/assets/scss/_vars.scss";
div .row {
  @include justify("between");
}

figure {
  width: 90px;
}

ul {
  @include center("y");

  a {
    font-weight: bold;
    padding: 10px;
    color: $dark-grey;
    &:hover {
      color: $blue;
    }
  }
}
</style>

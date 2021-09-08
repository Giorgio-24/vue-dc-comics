<template>
  <header class="container h-120">
    <div class="row">
      <figure class="clickable">
        <img src="@/assets/img/dc-logo.png" alt="dc-logo" class="img-fluid" />
      </figure>
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a
            class="uppercase"
            :class="link.current === true ? 'selected' : ''"
            @click="this.currentLink = index"
            :href="link.url"
            >{{ link.text }}</a
          >
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
      currentLink: 3,
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
      computed: {
        selectedLink() {
          /* if (index === this.currentLink) */
          this.links[this.currentLink].current === true;
        },
      },
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_mixins.scss";
@import "@/assets/scss/_vars.scss";

header {
  @include center("y");
}

div.row {
  width: 100%;
  @include justify("between");
}

figure {
  height: 90px;
  @include center("y");
}

ul {
  @include center("y");

  a {
    font-weight: bold;
    padding: 10px;
    color: $dark-grey;
    &.selected {
      color: $blue;
      border-bottom: 2px solid $blue;
    }
    &:hover {
      color: $blue;
      border-bottom: 2px solid $blue;
    }
  }
}
</style>

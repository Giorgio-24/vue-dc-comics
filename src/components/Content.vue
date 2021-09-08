<template>
  <section>
    <div class="container h-100">
      <div class="card" v-for="(card, index) in cards" :key="index">
        <figure>
          <img class="img-fluid" :src="card.thumb" :alt="card.series" />
        </figure>
        <div class="uppercase">{{ card.series }}</div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Content",
  props: ["cards"],
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_mixins.scss";
section {
  background-color: #1c1c1c;

  div.container {
    padding: 60px 0;
    display: flex;
    flex-wrap: wrap;
    .card {
      color: #fff;
      width: 160px;
      margin: 20px;
      figure {
        height: 160px;
      }
      div {
        margin-top: 10px;
      }
    }
  }
}
</style>
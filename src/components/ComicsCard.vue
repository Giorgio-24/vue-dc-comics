<template>
  <div>
    <div class="card clickable">
      <figure>
        <img class="img-fluid" :src="card.thumb" :alt="card.series" />
      </figure>
      <div class="uppercase">{{ card.series }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["card"],
};
</script>

<style lang="scss" scoped>
.card {
  color: #fff;
  width: 160px;
  margin: 20px;
  &:hover {
    position: relative;
    bottom: 10px;
  }
  figure {
    height: 160px;
  }
  div {
    margin-top: 10px;
  }
}
</style>
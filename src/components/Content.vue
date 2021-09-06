<template>
  <section class="h-120">
    <div class="container h-100">
      <h3 class="">--- Content goes here ---</h3>
    </div>
  </section>
</template>

<script>
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_mixins.scss";
section {
  background-color: #000;

  div.container {
    @include center("y");

    h3 {
      color: #fff;
      font-size: 25px;
      /*   @include center("y"); */
      align-self: center;
    }
  }
}
</style>
<template>
  <section>
    <div class="container h-100">
      <ul class="h-100">
        <li><a href="#">Digital comics</a></li>
        <li><a href="#">DC merchandise</a></li>
        <li><a href="#">Subscription</a></li>
        <li><a href="#">Comic shop locator</a></li>
        <li><a href="#">Dc power visa</a></li>
      </ul>
    </div>
  </section>
</template>

<script>
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
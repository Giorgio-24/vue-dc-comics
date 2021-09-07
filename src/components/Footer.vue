<template>
  <section>
    <div class="container h-100">
      <div class="">
        <a href="#" class="uppercase">Sign-up now!</a>
      </div>
      <div class="d-flex">
        <ul class="d-flex">
          <li><a href="#" class="uppercase">Follow us</a></li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-facebook.png" alt=""
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-twitter.png" alt=""
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-youtube.png" alt=""
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-pinterest.png" alt=""
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-periscope.png" alt=""
            /></a>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_mixins.scss";
@import "@/assets/scss/_vars.scss";

section {
  background-color: $dark-grey;
  width: 100%;
  height: 105px;
  position: fixed;
  top: calc(100% - 105px);
  z-index: 1;

  div.container {
    @include justify("between");
    @include center("y");

    > div:first-of-type {
      display: flex;
      a {
        color: #fff;
        border: 3px solid $blue;
        padding: 15px;
        font-weight: normal;
      }
    }
    ul {
      @include center("y");
    }
    a {
      padding: 0 10px;
      height: 100%;
      &.uppercase {
        color: $blue;
        font-weight: bold;
      }
    }
  }
}
</style>
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
              ><img src="../assets/img/footer-facebook.png" alt="facebook-logo"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-twitter.png" alt="twitter-logo"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-youtube.png" alt="youtube-logo"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img
                src="../assets/img/footer-pinterest.png"
                alt="pinterest-logo"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img
                src="../assets/img/footer-periscope.png"
                alt="periscope-logo"
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
      padding: 25px 10px;
      height: 100%;
      &.uppercase {
        color: $blue;
        font-weight: bold;
        &:hover {
          transform: scale(1.1);
          color: $blue;
        }
      }
      &:hover {
        filter: brightness(0) invert(1);
      }
    }
  }
}
</style>
<template>
  <section class="container">
    <div class="d-flex">
      <div>
        <h3 class="uppercase">Dc comics</h3>
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
        </ul>
        <h3 class="uppercase">Shop</h3>
        <ul>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
      </div>
      <div>
        <h3 class="uppercase">Dc</h3>
        <ul>
          <li><a href="#">Therms Of Use</a></li>
          <li><a href="#">Privacy Policy (New)</a></li>
          <li><a href="#">Ad Choiches</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>
      <div>
        <h3 class="uppercase">Sites</h3>
        <ul>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
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
  padding: 30px 0;

  > div {
    margin-bottom: 115px;
    div {
      margin: 0 15px;

      h3 {
        color: #fff;
        font-size: 22px;
        margin: 20px 0;
      }
    }
  }
}

li {
  padding: 5px 0;
  a {
    color: $lighter-grey;
    &:hover {
      color: #fff;
      border-bottom: 2px solid $blue;
    }
  }
}
</style>
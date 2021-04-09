<template>
  <div class="home-page">
    <Home />
    <About />
    <div class="index-bottom" />
  </div>
</template>

<style>
  .home-page {
    background-image: url("~assets/blossom-bg.png");
    background-size: 100vw auto;
    background-repeat: no-repeat;
  }

  .index-bottom {
    height: 36px;
    width: 100%;
    background-color: var(--main-navy);
  }

  @media (max-width: 767px) {
    .home-page {
      background-size: auto;
    }
  }
</style>

<script>
import Home from '~/components/home.vue'
import About from '~/components/about.vue'

export default {
  components: {
    Home,
    About
  }
}
</script>

<template>
  <div>
    <Home />
    <About />
    <div class="index-bottom" />
  </div>
</template>

<style>
  .index-bottom {
    height: 36px;
    width: 100%;
    background-color: var(--main-navy);
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

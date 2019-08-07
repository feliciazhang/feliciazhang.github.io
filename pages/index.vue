<template>
  <div>
    <ContactBar />
    <Nav />
    <Home />
    <About />
  </div>
</template>

<style>

</style>

<script>
import Nav from '~/components/nav.vue'
import ContactBar from '~/components/contact.vue'
import Home from '~/components/home.vue'
import About from '~/components/about.vue'

export default {
  components: {
    Nav,
    ContactBar,
    Home,
    About
  }
}
</script>

<template>
  <div>
    <ContactBar />
    <Nuxt />
  </div>
</template>

<script>
import ContactBar from '~/components/contact.vue'

export default {
  components: {
    ContactBar
  }
}
</script>

<style>
  :root {
    --font-montserrat: "Montserrat";
    --font-ovo: "Ovo";
    --main-navy: #283246;
    --main-pink: #f5cbcb;
    --main-neutral: #ffffff;
    --main-red: #b85e5e;
  }

  html {
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    scroll-behavior: smooth;
  }

  body {
    margin: 0;
    background: var(--main-neutral);
    color: var(--main-navy);
    font-family: var(--font-montserrat);
    font-size: 18px;
    line-height: 22px;
  }

  body * {
    box-sizing: border-box;
  }

  a,
  a:hover {
    color: var(--main-navy);
  }

  h2 {
    font-family: var(--font-ovo);
    font-size: 36px;
  }

  h3 {
    font-size: 24px;
  }

  @media (max-width: 767px) {
    body {
      font-size: 16px;
      line-height: 20px;
    }

    h2 {
      font-size: 24px;
    }

    h3 {
      font-size: 20px;
    }
  }
</style>

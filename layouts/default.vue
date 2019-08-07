<template>
  <div>
    <Nuxt />
  </div>
</template>

<style>
  @import url("https://fonts.googleapis.com/css?family=Montserrat|Ovo");

  :root {
    --font-montserrat: "Montserrat";
    --font-ovo: "Ovo";
    --main-navy: #283246;
    --main-pink: #f5cbcb;
    --main-neutral: #f7f0e9;
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
    font-size: 16px;
    line-height: 22px;
  }

  body * {
    box-sizing: border-box;
  }
</style>

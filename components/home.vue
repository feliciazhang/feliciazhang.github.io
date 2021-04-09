<template>
  <div class="home-container">
    <img class="home-portrait" src="~assets/felicia.jpeg" />
    <h1 class="home-title">
      felicia zhang
    </h1>
    <p>likes to make stuff</p>
  </div>
</template>

<style>
  .home-container {
    text-align: center;
    height: 100vh;
  }

  .home-portrait {
    width: 240px;
    height: 240px;
    border-radius: 50%;
    border: 2px solid var(--main-red);
    margin: 25vh 0 16px;
    box-shadow: 3px 3px 12px 3px #ccc;
  }

  .home-title {
    font-size: 32px;
    font-family: var(--font-ovo);
  }

  @media (max-width: 767px) {
    .home-container {
      height: auto;
    }
  }
</style>

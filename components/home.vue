<template>
  <div class="home-container">
    <img class="home-portrait" src="~assets/felicia.jpg" />
    <h1 class="home-title">
      felicia zhang
    </h1>
    <p>engineer, artist, and aiming to be much more</p>
  </div>
</template>

<style>
  .home-container {
    text-align: center;
    padding: 96px 48px 48px;
    height: 100vh;
    background-image: url("~assets/home-bg.png");
    background-size: cover;
  }

  .home-portrait {
    width: 240px;
    height: 240px;
    border-radius: 50%;
    border: 2px solid var(--main-red);
    margin: 0 0 16px;
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

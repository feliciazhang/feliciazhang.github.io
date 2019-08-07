<template>
  <div class="contact-bar-container">
    <ul class="contact-bar">
      <li class="contact-item">
        <a href="https://www.linkedin.com/in/feliciayzhang/" target="_blank">
          <img src="~assets/linkedin.svg" />
        </a>
      </li>

      <li class="contact-item">
        <a href="https://github.com/feliciazhang" target="_blank">
          <img src="~assets/git.svg" />
        </a>
      </li>
      <li class="contact-item">
        zhang.fel at husky.neu.edu
      </li>
    </ul>
  </div>
</template>

<style>
  .contact-bar-container {
    background-color: var(--main-neutral);
    width: 100%;
    position: fixed;
    top: 0;
  }

  .contact-bar {
    padding: 8px;
    float: right;
    list-style-type: none;
    margin: 0;
  }

  .contact-item {
    display: inline-block;
    padding: 4px;
    vertical-align: middle;
    font-family: var(--font-ovo);
  }
</style>

<template>
  <div class="contact-bar-container">
    <ul class="nav">
      <li
        v-for="item in navItems"
        :key="item.text"
        class="nav-item"
      >
        <a :href="item.link">
          {{ item.text }}
        </a>
      </li>
    </ul>

    <ul class="contact-bar">
      <li class="contact-item">
        <a href="https://www.linkedin.com/in/feliciayzhang/" target="_blank">
          <img src="~assets/icons/linkedin.svg" />
        </a>
      </li>

      <li class="contact-item">
        <a href="https://github.com/feliciazhang" target="_blank">
          <img src="~assets/icons/git.svg" />
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
    background-color: rgba(247,240,233, 0.5);
    width: 100%;
    position: fixed;
    top: 0;
    height: 54px;
  }

  .nav {
    list-style-type: none;
    box-shadow: none;
    float: left;
  }

  .nav-item {
    display: inline-block;
    margin: 0 16px;
    padding-bottom: 4px;
  }

  .nav-item a {
    text-decoration: none;
    color: var(--main-navy);
  }

  .nav-item:hover {
    border-bottom: 2px solid var(--main-navy);
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

<script>
export default {
  data: () => (
    {
      navItems: [
        { text: 'about', link: '/#about' },
        { text: 'what i do', link: '/#experience' },
        { text: "how i'm feeling", link: '/mood' }]
      // { text: 'gallery', link: '/gallery' }]
    }
  )
}
</script>

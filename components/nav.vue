<template>
  <div>
    <ul class="nav">
      <li
        v-for="item in navItems"
        :key="item.text"
        class="nav-item"
      >
        <a :href="item.link">
          <div class="nav-dot" />
        </a>
        <span class="nav-tag">{{ item.text }}</span>
      </li>
    </ul>
  </div>
</template>

<style>
  .nav {
    background-color: var(--main-navy);
    opacity: 0.6;
    padding: 0 8px;
    position: fixed;
    right: 0;
    top: 40%;
    border-radius: 4px 0 0 4px;
    transition: opacity 300ms ease;
    list-style-type: none;
    box-shadow: none;
  }

  .nav:hover {
    opacity: 1;
    box-shadow: 3px 3px 12px 6px #aaa;
  }

  .nav li {
    position: relative;
  }

  .nav-dot {
    width: 12px;
    height: 12px;
    margin: 16px 0;
    background-color: var(--main-neutral);
    border-radius: 50%;
    cursor: pointer;
  }

  .nav:hover .nav-dot {
    margin: 16px 24px 16px 0;
  }

  .nav-tag {
    opacity: 0;
    transition: opacity 300ms ease;
    position: absolute;
    left: -88px;
    width: 72px;
    top: calc(50% - 6px);
    font-size: 12px;
    text-align: right;
  }

  .nav-item:hover .nav-tag {
    opacity: 1;
  }
</style>

<script>
export default {
  data: () => (
    {
      navItems: [
        { text: 'about', link: '#about' },
        { text: 'what i do', link: '#experience' },
        { text: 'gallery', link: '/gallery' }]
    }
  )
}
</script>

<template>
  <div class="food">
    <ul class="food-list">
      <li
        v-for="item in foodSections"
        :key="item.title"
        class="food-list-item"
      >
        <span @click="selectedfood = item.id">{{ item.title }}</span>
      </li>
    </ul>

    <div class="food-content">
      <Welcome :class="[ selectedfood == 'welcome' ? 'food-content-active': '', 'food-content-section' ]" />
      <Batches :class="[ selectedfood == 'batches' ? 'food-content-active': '', 'food-content-section' ]" />
      <Bits :class="[ selectedfood == 'bits' ? 'food-content-active': '', 'food-content-section' ]" />
      <Fancy :class="[ selectedfood == 'fancy' ? 'food-content-active': '', 'food-content-section' ]" />
    </div>
  </div>
</template>

<style>
  .food {
    margin-top: 54px;
  }

  .food-list {
    height: calc(100vh - 54px);
    width: 250px;
    min-width: 250px;
    list-style-type: none;
    padding: 16px 24px;
    background-color: var(--main-navy);
    color: var(--main-neutral);
    margin: 0;
    position: fixed;
    bottom: 0;
  }

  .food-list-item {
    margin: 8px 0;
    cursor: pointer;
  }

  .food-list-item:hover {
    text-decoration: underline;
  }

  .food-content {
    padding: 48px 100px 48px 298px;
  }

  .food-content h1 {
    margin-top: 0;
  }

  .food-content-section {
    display: none;
  }

  .food-content-active {
    display: block;
  }
</style>

<script>
import Welcome from '~/components/food/welcome.vue'
import Batches from '~/components/food/batches.vue'
import Bits from '~/components/food/bits.vue'
import Fancy from '~/components/food/fancy.vue'

const foodData = [
  { title: 'welcome', id: 'welcome' },
  { title: 'easy batches', id: 'batches' },
  { title: 'bits', id: 'bits' },
  { title: '"fancy" stuff', id: 'fancy' }]

export default {
  components: {
    Welcome,
    Batches,
    Bits,
    Fancy
  },
  data: () => (
    {
      foodSections: foodData,
      selectedfood: foodData[0].id
    }
  )
}
</script>

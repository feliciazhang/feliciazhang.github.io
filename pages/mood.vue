<template>
  <div class="mood">
    <ul class="mood-list">
      <li
        v-for="item in moodboards"
        :key="item.title"
        :class="['mood-list-item', selectedMood.title == item.title ? 'selected-mood-item' : '']"
        @click="selectedMood = item"
      >
        <span>{{ item.title }}</span>
      </li>
    </ul>

    <img class="main-board" :src="require('../assets/mood/' + selectedMood.file)" />
  </div>
</template>

<style>
  .mood {
    margin-top: 54px;
    display: flex;
    overflow: hidden;
    background-color: var(--main-neutral);
  }

  .mood-list {
    height: calc(100vh - 54px);
    overflow-y: auto;
    width: 250px;
    min-width: 250px;
    list-style-type: none;
    padding: 16px 0;
    background-color: var(--main-navy);
    color: var(--main-neutral);
    margin: 0;
  }

  .selected-mood-item {
    background-color: var(--main-neutral);
    color: var(--main-navy);
  }

  .mood-list-item {
    padding: 8px 24px;
    cursor: pointer;
  }

  .mood-list-item:hover {
    text-decoration: underline;
  }

  .main-board {
    height: 85vh;
    margin: auto;
  }
</style>

<script>
import moodData from '~/assets/mood.json'

export default {
  data: () => (
    {
      moodboards: moodData,
      selectedMood: moodData[0]
    }
  )
}
</script>

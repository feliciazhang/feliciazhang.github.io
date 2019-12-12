<template>
  <div class="mood">
    <ul class="mood-list">
      <li
        v-for="item in moodboards"
        :key="item.title"
        class="mood-list-item"
      >
        <span @click="selectedMood = item">{{ item.title }}</span>
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
  }

  .mood-list {
    height: calc(100vh - 54px);
    overflow-y: auto;
    width: 250px;
    list-style-type: none;
    padding: 16px 24px;
    background-color: var(--main-navy);
    color: var(--main-neutral);
    margin: 0;
  }

  .mood-list-item {
    margin: 4px 0;
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

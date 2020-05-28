<template>
  <div>
    <h1>easy batches</h1>
    <p>
      why wash more than one pot? these are the easiest things to make and you get a bunch of meals out of it. ideal for family dinner. the main categories here are stirfry, curry, pastas, and stews/soups.
    </p>
    <div class="batch-section">
      <div class="batch-section-title" v-on:click="stirfryExpand = !stirfryExpand">
        <h2>stirfry</h2>
        <img src="~assets/icons/arrow.svg" />
      </div>
      <div v-if="stirfryExpand" class="batch-section-content">
        this is called u cook the same thing for family dinner multiple times with slight modifications and pretend it's a different meal. just add rice or noodles, veggies of your choice, eggs or tofu as protein if you so desire, and a sauce.
        <h5>sauces (i dont know any quantities sorry just taste)</h5>
        <ul>
          <li>literally just soy sauce (sad stirfry)</li>
          <li><b>peanut sauce:</b> peanut butter & soy sauce & brown sugar | honey & ginger powder</li>
          <li><b>lao mian sauce:</b> soy sauce & garlic chili sauce & hoisin & sesame oil & rice vinegar</li>
          <li><b>the low effort one:</b> hoisin & soy sauce & lao gan ma</li>
        </ul>
        peanut sauce is really good w pad thai style rice noodles and vietnamese fresh rolls and the last sauce is good with ramen noodles.<br/><br/>
        if you're using egg you can scramble it in, or if you're lazy just fry one and stick it on top. and it'll look fancy.
      </div>
    </div>

    <div class="batch-section">
      <div class="batch-section-title" v-on:click="curryExpand = !curryExpand">
        <h2>curry</h2>
        <img src="~assets/icons/arrow.svg" />
      </div>
      <div v-if="curryExpand" class="batch-section-content">
        another one of those use new vegetables and pretend it's different type deals. if you're using potato or carrot or something that takes a long time to cook, it helps to half boil them before adding them with everything else. potato + carrot + celery is good with golden curry. anything is good. curry is good. I've never made a good thai curry though but that's why we can get takeout. <a href="https://simpleveganblog.com/vegetable-curry/" target="_blank">this one</a> is really good but the veggies are weird. try potato, cauliflower, bell pepper, spinach.
      </div>
    </div>

    <a data-pin-do="embedBoard" data-pin-board-width="865" data-pin-scale-height="240" data-pin-scale-width="865" href="https://www.pinterest.com/16fyz/michelin/easy-batch/"></a>
    <script async defer src="//assets.pinterest.com/js/pinit.js"></script>
  </div>
</template>

<style>
.batch-section {
  margin: 16px 0;
}

.batch-section-title {
  width: 100%;
  background-color: var(--main-navy);
  color: var(--main-neutral);
  display: flex;
  justify-content: space-between;
  padding: 8px 16px;
  border-radius: 4px;
  cursor: pointer;
  margin-bottom: 16px;
}

.batch-section-title h2 {
  margin: 0;
}

.batch-section-title img {
  width: 24px;
}

.batch-section-content {
  padding: 0 12px;
}
</style>

<script>
export default {
  name: 'Batches',
  data: () => (
    {
      stirfryExpand: false,
      curryExpand: false
    }
  )
}
</script>

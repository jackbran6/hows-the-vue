<template>
  <div class="card" :class="{ secondary: check }">
    <div v-if="!closed" class="open-section">
      <nuxt-link :to="route" class="title">{{ title }}</nuxt-link>
      <p class="contact">{{ contact }}</p>
      <p class="weekday-hours">Mon-Fri {{ weekdays }}</p>
      <p class="weekend-hours">Sat/Sun {{ weekend }}</p>
    </div>
    <div v-else class="closed">
      <nuxt-link :to="route" class="title">{{ title }}</nuxt-link>
      <p class="contact">{{ contact }}</p>
      <p class="weekday-hours">Mon-Fri {{ weekdays }}</p>
      <p class="weekend-hours">Sat/Sun {{ weekend }}</p>
      <nuxt-link :to="route" class="title">{{ title }}</nuxt-link>
      <p class="contact">{{ contact }}</p>
      <p class="weekday-hours">Mon-Fri {{ weekdays }}</p>
      <p class="weekend-hours">Sat/Sun {{ weekend }}</p>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'ContactBox',
  props: {
    route: {
      type: String,
      default: ''
    },
    title: {
      type: String,
      default: 'Contact'
    },
    contact: {
      type: String,
      default: 'whatsup.co.nz'
    },
    weekdays: {
      type: String,
      default: '12pm-3pm'
    },
    weekend: {
      type: String,
      default: '12pm-3pm'
    },
    check: {
      type: Boolean,
      default: false
    },
    closed: {
      type: Boolean,
      default: false
    }
  }
})
</script>

<style scoped>
.card {
  background: #c5e8e8;
  display: flex;
  flex-direction: column;
  padding: 100px 50px;
}
.title {
  font-size: 30px;
  text-decoration: none;
}
.secondary {
  background: #adbaea;
}
</style>

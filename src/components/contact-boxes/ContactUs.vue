<template>
<div class="card">
  <h3>{{title}}</h3>
  <h4 class="contact">{{contact}}</h4>
  <p class="weekday-hours">Mon-Fri {{weekdays}}</p>
  <p class="weekend-hours">Sat/Sun {{weekend}}</p>
</div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'ContactBox',
  props: {
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
  }
})
</script>

<style scoped>
.card {
  background-color: rgb(210, 255, 192);
  display: flex;
  flex-direction: column;
  padding: 30px;

}
</style>

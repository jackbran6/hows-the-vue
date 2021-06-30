<template>
  <div class="container">
    <Partners />
    <Promote />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

import Partners from '@/components/partners/Partners.vue'
import Promote from '@/components/promote/Promote.vue'
export default Vue.extend({
  name: 'PartnerPromotions',
  components: {
    Partners,
    Promote
  }
})
</script>

<style scoped>
.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  margin: auto;
}
</style>

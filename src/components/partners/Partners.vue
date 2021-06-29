<template>
  <div class="content-container">
    <p class="partners">
      Our amazing partners are
      <a class="partners" href="https://milfordasset.com/"
        >Milford Asset Management</a
      >, the
      <a
        class="partners"
        href="https://www.mediaworks.co.nz/home/about/mediaworks-foundation.html"
        >MediaWorks Foundation</a
      >
      and <a class="partners" href="https://www.officemax.co.nz/">Office Max</a>
    </p>
    <p class="learn">Learn more about our partners</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'Partners',
  props: {
    content: {
      type: String,
      default: 'This is default content'
    }
  }
})
</script>

<style scoped>
.content-container {
  background: #8f8cb2;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 200px 50px 50px;
}
.partners {
  font-size: 2rem;
  font-weight: 600;
}
.learn {
  justify-self: flex-end;
}
</style>

<template>
  <div class="header"><MenuButton class="hamburger" /></div>
</template>

<script lang="ts">
import Vue from 'vue'
import MenuButton from '@/components/menu-button/MenuButton.vue'
export default Vue.extend({
  name: 'Header',
  components: {
    MenuButton
  }
})
</script>

<style lang="scss" scoped>
@import '~assets/styles/config';

.header {
  @include type(14px, 18px);

  display: flex;
  justify-content: flex-end;
  padding-right: 20px;
  padding-top: 40px;
  position: absolute;
  width: 100%;
}
</style>

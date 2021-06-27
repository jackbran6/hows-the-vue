<template>
  <Intro>
    <Heading content="hows-the-vue" />
    <p>
      Welcome to the
      <a
        href="https://formfunfunction.com/"
        target="_blank"
        rel="noreferrer"
      >formfunfunction</a>
      Nuxt starter project. Head to<Code>/src/pages/index.vue</Code> to get
      stuck in.
    </p>
    <nuxt-link class="about-button" to="/about" >About</nuxt-link>
  </Intro>

</template>
<script lang="ts">
import Vue from 'vue'
import Intro from '@/components/intro/Intro.vue'
import Code from '@/components/intro/Code.vue'
import Heading from '@/components/intro/Heading.vue'

export default Vue.extend({
  name: 'Home',
  components: {
    Intro,
    Code,
    Heading
  },

  head: {
    title: 'Hello world!'
  }
})
</script>

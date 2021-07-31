<template>
  <div>
    <Header />
    <nuxt />
  </div>
</template>

<script lang="ts">
import { defineComponent } from '@nuxtjs/composition-api'
import Header from '@/components/Header.vue'

export default defineComponent({
  name: 'Layout',
  components: {
    Header,
  },
  setup() {},
})
</script>

<style lang="scss" scoped>
</style>

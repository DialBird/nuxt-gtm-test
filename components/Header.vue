<template>
  <header class="h-16 border-b">
    <div class="container h-full mx-auto flex items-center gap-4">
      <nuxt-link to="/">Home</nuxt-link>
      <nuxt-link to="/about">About</nuxt-link>
      <nuxt-link to="/works">Works</nuxt-link>
    </div>
  </header>
</template>

<script lang="ts">
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
  name: 'Header',
  setup() {},
})
</script>

<style lang="scss" scoped>
</style>

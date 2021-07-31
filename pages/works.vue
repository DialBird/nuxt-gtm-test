<template>
  <div class="container mx-auto mt-4">
    <h1 class="text-xl font-bold">Works</h1>
    <button
      class="
        bg-blue-500
        hover:bg-blue-700
        text-white
        font-bold
        py-2
        px-4
        rounded
      "
      @click="onClick"
    >
      Click
    </button>
  </div>
</template>

<script lang="ts">
import { defineComponent, useContext } from '@nuxtjs/composition-api'

export default defineComponent({
  name: '',
  setup() {
    const { $gtm } = useContext()
    const onClick = () => {
      $gtm.push({ event: 'click works!' })
    }

    return { onClick }
  },
})
</script>

<style lang="scss" scoped>
</style>

<template>
  <div class="container mx-auto mt-4">
    <Tutorial />
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
      @click="clickEvent"
    >
      Click
    </button>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  methods: {
    clickEvent() {
      console.log(this)
      this.$gtm.push({ event: 'demo' })
    },
  },
})
</script>

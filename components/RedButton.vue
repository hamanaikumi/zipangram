<template>
  <button
    class="inline-flex justify-center py-2 px-4 text-xl text-warning-color font-semibold"
    @click="onClick"
  >
    {{ name }}
  </button>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  props: {
    name: { type: String, required: true },
  },
  methods: {
    onClick() {
      this.$emit('emit')
    },
  },
})
</script>

<style></style>

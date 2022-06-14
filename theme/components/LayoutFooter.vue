<script setup lang="ts">
import { defineProps, computed } from 'vue'
import { useNow } from '@vueuse/core'

const props = defineProps({
  eventLogo: {
    type: String,
  },
  eventUrl: {
    type: String,
  },
  author: {
    type: String,
  },
  authorUrl: {
    type: String,
  },
})

const { now } = useNow()

const date = computed(() => now?.value.toLocaleDateString('en-US'))
</script>
<template>
  <footer
    v-if="eventLogo || author"
    class="
      mt-auto
      flex
      justify-between
      items-center
      w-full
      text-primary
      dark:text-white
      z-10
    "
  >
    <div class="mb-0 flex items-center">
      <!-- <a v-if="eventLogo" :href="eventUrl" target="_blank"
        ><img v-if="eventLogo" :src="eventLogo" class="h-8 mr-4" alt="Event image" /></a
      > -->
      <span>{{ date }}</span>
    </div>
    <a v-if="author" :href="authorUrl" target="_blank">{{ author }}</a>
  </footer>
</template>

<style scoped>
a {
  border-color: transparent;
}
</style>

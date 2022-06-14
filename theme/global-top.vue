<!-- global-top.vue -->

<template>
  <footer
    v-if="$slidev.themeConfigs.eventLogo || $slidev.themeConfigs.author"
    class="absolute bottom-0 p-4 mt-auto flex justify-between items-center w-full text-primary dark:text-white z-10"
  >
    <div class="mb-0 flex items-center">
      <a
      v-if="$slidev.themeConfigs.eventLogo" 
      :href="$slidev.themeConfigs.eventUrl" target="_blank"
        ><img
          :src="$slidev.themeConfigs.eventLogo"
          class="h-8 mr-4"
          alt="Event image"
      /></a>
    </div>
    <a
      v-if="$slidev.themeConfigs.author"
      :href="$slidev.themeConfigs.authorUrl"
      target="Presenter"
      >{{ $slidev.themeConfigs.author }}</a
    >
  </footer>
</template>

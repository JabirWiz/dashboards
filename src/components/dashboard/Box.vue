<script setup>
const props = defineProps(['pillBg', 'pillColor', 'date', 'title', 'description'])
</script>

<template>
  <div class="bg-white pa-4 d-flex rounded-lg ga-4 w-100">
    <div class="rounded-xl d-flex align-end" style="width: 10px;" :style="{background: pillBg}">
      <div class="rounded-xl" style="width: 10px; height: 65%;" :style="{background: pillColor}"></div>
    </div>
    <div class="">
      <p class="text-body-2 text-grey-darken-1 mb-1">{{ date }}</p>
      <h3>{{ title }}</h3>
      <p class="text-body-2 text-grey-darken-1 mt-1">{{ description }}</p>
    </div>
  </div>
</template>
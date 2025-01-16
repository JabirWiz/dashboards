<script setup>
const props = defineProps(['title', 'time1', 'time2', 'color', 'width'])
</script>

<template>
  <div class="border rounded-xl pa-4 my-4">
    <div class="d-flex justify-space-between ">
      <p class="font-weight-bold">{{ title }}</p>
      <p><span class="font-weight-bold">{{ time1 }}</span> <span v-if="time2">/ {{ time2 }}</span> hrs</p>
    </div>
    <div class="w-100 bg-blue-grey-lighten-5 mt-2 rounded-xl" style="height: 5px;">
      <div class="rounded-xl" style="height: 5px;" :class="color, width"></div>
    </div>
  </div>
</template>
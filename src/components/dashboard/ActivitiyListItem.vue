<script setup>
const porps = defineProps(['activity', 'time']);
</script>

<template>
  <li class="d-flex ga-4 mb-8">
    <span class="border-lg rounded-circle position-absolute bg-white" style="left: -10px; width: 18px; height: 18px; border-color: #81C784 !important;"></span>
    <div class="ml-8">
      <h4 class="font-weight-bold" style="line-height: 0%;">{{ activity }}</h4>
      <p class="text-grey mt-2">{{ time }}</p>
    </div>
  </li>
</template>
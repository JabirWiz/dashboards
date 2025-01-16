<script setup>
import ActivitiyListItem from './ActivitiyListItem.vue';

</script>

<template>
  <div class="border rounded-xl pa-4">

    <h4 class="text-blue font-weight-bold">Today Activity</h4>


    <ul class="mt-8 ml-4 border-s position-relative">
      <ActivitiyListItem :activity="'Punched In at'" :time="'10.00 AM.'" />
      <ActivitiyListItem :activity="'Punched Out at'" :time="'11.00 AM.'" />
      <ActivitiyListItem :activity="'Punched In at'" :time="'11.30 AM.'" />
      <ActivitiyListItem :activity="'Punched Out at'" :time="'01.30 AM.'" />
      <ActivitiyListItem :activity="'Punched In at'" :time="'02.30 AM.'" />
      <ActivitiyListItem :activity="'Punched Out at'" :time="'07.00 AM.'" />
    </ul>
  </div>
</template>
<script setup>
import StatisticsSlider from './StatisticsSlider.vue';
</script>


<template>
  <div class="border rounded-xl pa-4">
    <h4 class="text-blue font-weight-bold">Statistics</h4>
    <StatisticsSlider :color="'bg-green-lighten-2'" :time1="'3.45'" :time2="'8'" :title="'Today'" :width="'w-50'" />
    <StatisticsSlider :color="'bg-red-lighten-2'" :time1="'28'" :time2="'40'" :title="'This Week'" :width="'w-33'" />
    <StatisticsSlider :color="'bg-orange-lighten-2'" :time1="'90'" :time2="'160'" :title="'This Month'" :width="'w-66'" />
    <StatisticsSlider :color="'bg-blue-lighten-1'" :time1="'90'" :time2="'160'" :title="'Remaining'" :width="'w-66'" />
    <StatisticsSlider :color="'bg-yellow-lighten-1'" :time1="'5'" :title="'Overtime'" :width="'w-25'" />
  </div>
</template>
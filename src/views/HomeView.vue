<script setup>
import AttendanceList from '@/components/dashboard/AttendanceList.vue';
import DailyRecords from '@/components/dashboard/DailyRecords.vue';
import Statistics from '@/components/dashboard/Statistics.vue';
import Timesheet from '@/components/dashboard/Timesheet.vue';
import TodayAcitivity from '@/components/dashboard/TodayAcitivity.vue';

</script>

<template>
  <div class="pa-10 w-100">

    <h2>Attendance</h2>
    <h3>Dashboard / Attendance</h3>

    <div class="d-flex w-100 my-10 ga-10">
      <Timesheet class="w-33" />
      <Statistics class="w-33" />
      <TodayAcitivity class="w-33" />
    </div>

    <div class="d-flex w-100 my-10 ga-10">
      <AttendanceList class="w-66" />
      <DailyRecords class="w-33" />
    </div>
  </div>
</template>

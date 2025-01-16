<script setup>
import { Chart as ChartJS, ArcElement, Tooltip, Legend } from 'chart.js'
import { Bar, Doughnut } from 'vue-chartjs'

ChartJS.register(ArcElement, Tooltip, Legend)

const data = {
  datasets: [{
    data: [55, 45],
    backgroundColor: [
      '#2196F3',
      'lightgray',
    ],
    hoverOffset: 4
  }]
};
const options = {
  responsive: false, // Disable responsiveness if you want fixed dimensions
  maintainAspectRatio: false, // Allow height and width to be independently set
  // width: 100,
  // height: 100,
  cutout: 70,
}
</script>

<template>
  <div class="border rounded-xl d-flex flex-column justify-space-between">
    <div class="pa-4">

      <h4 class="text-blue font-weight-bold">Timesheet <span class="text-grey ms-2">11 Mar 2019</span></h4>
      <div class="border rounded-xl pa-4 my-4">
        <p class="font-weight-bold">Punch in at</p>
        <p class="text-grey">Wed, 11th Mar 2019 10.00 AM</p>
      </div>

      <div class="position-relative d-flex align-center justify-center" style="z-index: 0;">
        <Doughnut :data="data" :options="options" class="" width="180" height="180" />
        <h3 class="text-h5 position-absolute">3.4 hrs</h3>
      </div>

      <div class="text-center my-4">
        <button class="border bg-green-lighten-4 px-10 py-2 rounded-lg mx-auto">Punch Out</button>
      </div>
    </div>

    <div class="d-flex border-t mt-auto">
      <button class="w-100 py-1">
        Break
        <br>
        1.21 hrs
      </button>
      <button class="w-100 border-s py-1">
        Overtime
        <br>
        3 hrs
      </button>
    </div>
  </div>
</template>
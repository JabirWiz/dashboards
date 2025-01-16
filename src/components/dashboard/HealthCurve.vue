<script setup>
import {
  Chart as ChartJS,
  CategoryScale,
  LinearScale,
  PointElement,
  LineElement,
  Title,
  Tooltip,
  Legend,
  Filler
} from 'chart.js'
import { Line } from 'vue-chartjs'

ChartJS.register(
  CategoryScale,
  LinearScale,
  PointElement,
  LineElement,
  Title,
  Tooltip,
  Legend,
  Filler
)

const data = {
  labels: ['January', 'February', 'March', 'April', 'May', 'June', 'July'],
  datasets: [
    {
      label: 'Data One',
      backgroundColor: 'rgba(8, 155, 171, 0.4)',
      data: [40, 39, 10, 40, 39, 80, 40],
      lineTension: 0.3,
      borderColor: ["#089bab"],
      fill: true,
      // backgroundColor: 'pink'
    }
  ]
}

const options = {
  responsive: true,
  maintainAspectRatio: true,
  plugins: {
    legend: {
      display: false
    }
  },
  scales: {
    x: {
      grid: {
        display: false,
      },
      border: {
        display: false,
      }
    },
  },
  // bezierCurve: true
}

</script>

<template>
  <div class="bg-white pa-4 rounded-lg">
    <h4 class="mb-4">Health Curve</h4>
    <Line :data="data" :options="options" height="100px" />
  </div>
</template>
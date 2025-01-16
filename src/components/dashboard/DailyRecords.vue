<script setup>
import {
  Chart as ChartJS,
  Title,
  Tooltip,
  Legend,
  BarElement,
  CategoryScale, LinearScale
} from 'chart.js'
import { Bar } from 'vue-chartjs'

ChartJS.register(CategoryScale, LinearScale, BarElement, Title, Tooltip, Legend)

const data = {
  labels: [
    '29',
    '30',
    '01',
    '02',
    '03',
    '04',
    '05',
    '06',
  ],
  datasets: [
    {
      label: 'Data One',
      backgroundColor: '#81C784',
      data: [30, 20, 5, 39, 90, 50, 30, 20],
      borderRadius: 20,
      borderSkipped: false,
      borderWidth: 1,
      categoryPercentage: 1.0,
      barPercentage: 0.5,
    },
    {
      categoryPercentage: 1.0,
      barPercentage: 0.5,
      label: 'Data Two',
      backgroundColor: '#2196F3',
      data: [100, 70, 52, 24, 34, 20, 60, 90],
      borderRadius: 20,
      borderSkipped: false,
    }
  ]
};
const options = {
  responsive: false,
  maintainAspectRatio: false,
  plugins: {
    legend: {
      display: false
    }
  },
  barThickness: 7,
  scales: {
    x: {
      grid: {
        display: false,
      },
      border: {
        display: false,
      }
    },
    y: {
      display: false,
    },
  }
}
</script>

<template>
  <div class="border rounded-xl d-flex flex-column justify-space-between pa-4">
    <h4 class="text-blue font-weight-bold">Daily Records</h4>

    <Bar :data="data" :options="options" />
  </div>
</template>
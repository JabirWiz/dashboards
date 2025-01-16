<script setup>

const attendanceList = [
  { no: 1, date: '19 Feb 2019', punchIn: '10 AM', punchOut: '7 PM', production: '9 hrs', break: '1 hrs', overtime: '2 hrs', },
  { no: 2, date: '19 Feb 2019', punchIn: '10 AM', punchOut: '7 PM', production: '9 hrs', break: '1 hrs', overtime: '2 hrs', },
  { no: 3, date: '19 Feb 2019', punchIn: '10 AM', punchOut: '7 PM', production: '9 hrs', break: '1 hrs', overtime: '2 hrs', },
  { no: 4, date: '19 Feb 2019', punchIn: '10 AM', punchOut: '7 PM', production: '9 hrs', break: '1 hrs', overtime: '2 hrs', },
  { no: 5, date: '19 Feb 2019', punchIn: '10 AM', punchOut: '7 PM', production: '9 hrs', break: '1 hrs', overtime: '2 hrs', },
  { no: 6, date: '19 Feb 2019', punchIn: '10 AM', punchOut: '7 PM', production: '9 hrs', break: '1 hrs', overtime: '2 hrs', },
]
</script>

<template>
  <div class="rounded-xl border overflow-hidden" style="border-collapse: collapse;">
    <h4 class="text-blue font-weight-bold pa-4">Attendance List</h4>
    <table class="table w-100 border" style="border-collapse: collapse;">
      <thead>
        <tr>
          <th>S.No</th>
          <th>Date</th>
          <th>Punch In</th>
          <th>Punch out</th>
          <th>Production</th>
          <th>Break</th>
          <th>Overtime</th>
        </tr>
      </thead>
      <tbody class="text-grey">
        <tr v-for="attendance in attendanceList" :key="attendance.no">
          <td>{{ attendance.no }}</td>
          <td>{{ attendance.date }}</td>
          <td>{{ attendance.punchIn }}</td>
          <td>{{ attendance.punchOut }}</td>
          <td>{{ attendance.production }}</td>
          <td>{{ attendance.break }}</td>
          <td>{{ attendance.overtime }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style scoped>
tr,
th,
td {
  border: 1px solid rgba(0, 0, 0, 0.12);
  text-align: center;
  padding: 10px;
}

th {
  font-weight: bold;
}
</style>
<script setup>
import { VCalendar } from 'vuetify/labs/VCalendar'
import Box from '@/components/dashboard/Box.vue';
import DoctorComponent from '@/components/dashboard/DoctorComponent.vue';
import HealthCurve from '@/components/dashboard/HealthCurve.vue';


</script>

<template>
  <div class="w-100 h-100 pa-6 d-flex flex-column ga-6" style="background: #eef7f8;">
    <div class="d-flex ga-6">
      <Box :pillBg="'rgb(205.6, 235, 238.2)'" :pillColor="'#089bab'" :title="'Hypertensive Crisis'" :date="'10 Feb, 2020'" :description="'Ongoing Treatment'" />
      <Box :pillBg="'rgb(251, 221.4, 221.4)'" :pillColor="'#eb5757'" :title="'Osteoporosis'" :date="'12 Jan, 2020'" :description="'Incurable'" />
      <Box :pillBg="'rgb(252.2, 225.2, 209.4)'" :pillColor="'#f16a1b'" :title="'Hypertensive Crisis'" :date="'15 Feb, 2020'" :description="'Examination'" />

      <div class="bg-white pa-4 d-flex rounded-lg ga-4 w-100">
        <img src="@/assets/img/box-img.png" alt="" srcset="" class="mx-auto" style="height: 112px;">
      </div>
    </div>

    <div class="d-flex ga-6">
      <DoctorComponent class="w-33" />
      <HealthCurve class="w-66" />
    </div>

    <div class="d-flex ga-6">
      <div class="w-33">
        <v-row>
          <v-col>
            <v-sheet>
              <v-calendar ></v-calendar>
            </v-sheet>
          </v-col>
        </v-row>
      </div>
    </div>

  </div>
</template>

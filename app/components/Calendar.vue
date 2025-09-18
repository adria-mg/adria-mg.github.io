<script setup lang="ts">
import { CalendarDate } from '@internationalized/date';
import { shallowRef } from 'vue';

const valores = shallowRef([
  new CalendarDate(2025, 9, 10),
  new CalendarDate(2025, 9, 11),
  new CalendarDate(2025, 9, 12),
  new CalendarDate(2025, 9, 13),
  new CalendarDate(2025, 9, 14),
  new CalendarDate(2025, 10, 25),
  new CalendarDate(2025, 10, 26),
  new CalendarDate(2025, 11, 29),
  new CalendarDate(2025, 11, 30),
  new CalendarDate(2025, 12, 18),
  new CalendarDate(2025, 12, 19),
  new CalendarDate(2025, 12, 20),
  new CalendarDate(2025, 12, 21),
  new CalendarDate(2025, 12, 22)
])
</script>

<template>
    <h3 class="text-2xl font-bold py-4 text-blue">Calendario de regatas</h3>
      <UCard class="bg-white text-red">   
        <UCalendar multiple v-model="valores" readonly :weekStartsOn="1"/>
      </UCard>
</template> 
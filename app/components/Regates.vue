<script setup>
  import Ranquing from './Ranquing.vue';
  import Calendar from './Calendar.vue';
  import ProxRegata from './ProxRegata.vue';
  import RegatasAutonomicas from './RegatasAutonomicas.vue';
  import BarcosVenta from './BarcosVenta.vue';

  let barcos = ['winner', 'osis', 'sailtech'];

</script>

<template>
  <div class="grid lg:grid-cols-8 gap-4 md:grid-cols-1 bg-toolightblue p-4">
    <div class="lg:col-start-2 lg:col-span-3 md:col-start-1">
      <Ranquing></Ranquing>
      <RegatasAutonomicas></RegatasAutonomicas>
    </div>
    <div class="lg:col-span-3">
        <Calendar></Calendar>
        <ProxRegata></ProxRegata>
    </div>
      </div>
    <div class="">
      <NuxtImg src="/bannersup.jpg" alt="logo" class="w-full"/>
    </div>
    <div class="grid lg:grid-cols-8 gap-4 md:grid-cols-1 bg-lightblue p-4">
      <div class="lg:col-start-2 lg:col-span-3">
        <News></News>
        </div>
        <div class="lg:col-span-3">
        <h3 class="text-2xl font-bold py-4 text-blue">Barcos en venta</h3>
        <div class="grid col-rows-3 gap-2" >
          <div class='col-row-1'  v-for="barco in barcos" :key="barco">
            <BarcosVenta v-bind:tipo-barco="barco"></BarcosVenta>
          </div>
        </div>
        </div>
    </div>
    


</template>

<style>
.mdi--location {
  display: inline-block;
  width: 24px;
  height: 24px;
  background-repeat: no-repeat;
  background-size: 100% 100%;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath fill='%23ff4c4c' d='M12 11.5A2.5 2.5 0 0 1 9.5 9A2.5 2.5 0 0 1 12 6.5A2.5 2.5 0 0 1 14.5 9a2.5 2.5 0 0 1-2.5 2.5M12 2a7 7 0 0 0-7 7c0 5.25 7 13 7 13s7-7.75 7-13a7 7 0 0 0-7-7'/%3E%3C/svg%3E");
}

.solar--calendar-bold {
  display: inline-block;
  width: 24px;
  height: 24px;
  background-repeat: no-repeat;
  background-size: 100% 100%;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath fill='%23ff4c4c' d='M7.75 2.5a.75.75 0 0 0-1.5 0v1.58c-1.44.115-2.384.397-3.078 1.092c-.695.694-.977 1.639-1.093 3.078h19.842c-.116-1.44-.398-2.384-1.093-3.078c-.694-.695-1.639-.977-3.078-1.093V2.5a.75.75 0 0 0-1.5 0v1.513C15.585 4 14.839 4 14 4h-4c-.839 0-1.585 0-2.25.013z'/%3E%3Cpath fill='%23ff4c4c' fill-rule='evenodd' d='M2 12c0-.839 0-1.585.013-2.25h19.974C22 10.415 22 11.161 22 12v2c0 3.771 0 5.657-1.172 6.828S17.771 22 14 22h-4c-3.771 0-5.657 0-6.828-1.172S2 17.771 2 14zm15 2a1 1 0 1 0 0-2a1 1 0 0 0 0 2m0 4a1 1 0 1 0 0-2a1 1 0 0 0 0 2m-4-5a1 1 0 1 1-2 0a1 1 0 0 1 2 0m0 4a1 1 0 1 1-2 0a1 1 0 0 1 2 0m-6-3a1 1 0 1 0 0-2a1 1 0 0 0 0 2m0 4a1 1 0 1 0 0-2a1 1 0 0 0 0 2' clip-rule='evenodd'/%3E%3C/svg%3E");
}
</style>
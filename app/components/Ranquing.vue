<script setup>
const position = [1, 2, 3, 4, 5];

const sailors = ['Adria Morata', 'Lluis Morata', 'Pau Mora', 'Jordi Camos', 'Ramon Figueras'];



</script>

<template>
    <h3 class="text-2xl font-bold py-4 text-blue">Ranking nacional</h3>
      <table class="table-auto border-separate bg-white border border-black rounded-lg shadow-sm w-full">
        <tbody class="border  border-gray-300">
          <tr
            class="odd:first:bg-yellow-500 odd:first:hover:bg-red hover:text-white text-black even:bg-gray-200 border-gray-300 rounded-sm border-separate hover:bg-red"
            v-for="(sailor, index) in sailors" :key="sailor">
            <td class="px-2 py-1.5 font-medium text-3xl" >{{ position[index] }}</td>
            <td class="px-1 py-1.5">
              <div class="grid grid-cols-6 items-center">
                <div class="ml-2 col-span-1">
                  <UAvatar v-bind:alt="sailor" size="xl" />
                </div>
                <div class="col-span-5 pl-2">
                  <p class="font-medium text-xl text-black">{{ sailor }}</p>
                  <p class="font-thin text-gray-600 text-2sm"> Club Vela Palamós</p>
                </div>
              </div>
            </td>
            <td class="px-1 py-1.5 font-regular text-black" >100</td>
          </tr>
        </tbody>
      </table>
</template>
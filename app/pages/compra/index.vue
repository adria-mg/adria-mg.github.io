<script setup lang="ts">
    let barcos = ['h', 'a', 'b', 'f', 'i'];
</script>

<template>
    <div class="grid lg:grid-cols-8 gap-4 md:grid-cols-1">
        <div class="col-start-2 col-span-6">
            <h3 class="text-5xl font-bold py-4 text-white">Barcos en venta:</h3>
            <div class="grid col-rows-10 gap-2" >
                <div class='col-row-1' v-for="barco in barcos" :key="barco">
                    <BarcosVenta v-bind:tipo-barco="barco"></BarcosVenta>
                </div>
            </div>
        </div>
    </div>

    <h3 class="text-2xl font-bold py-4 text-blue">¿Quieres vender tu barco?</h3>
</template>
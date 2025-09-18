<script setup>
    const props = defineProps({
        tipoBarco: String
    });

</script>

<template>
    <UCard class="bg-white">
        <div class="grid grid-cols-3 gap-4">
            <div class="col-span-1">
                <NuxtImg src="/LogoEuropeCat_2025.png" alt="logo" class="w-full"/>
            </div>
            <div class="col-span-2">
                <h5 class="text-black font-semibold text-xl">Barco {{ tipoBarco }} 2025 </h5>
                <p class="text-gray-500 font-regular">Hola a todos vendo un barco.</p>
            </div>
        </div>
    </UCard>
</template>

<script setup>
defineProps({
  details: Object,
});
</script>

<template>
  <div
    class="ps-5 pe-5 py-3 m-3 bg-white border border-gray-200 rounded-lg shadow w-1/3"
  >
    <div class="flex justify-between">
      <div class="flex items-center pe-14">
        <i :class="details.icon" class="pe-5 text-2xl"></i>
        <p class="text-xl font-bold text-gray-500">{{ details.name }}</p>
      </div>
      <i class="bi bi-grid text-blue-600"></i>
    </div>

    <h5 class="my-5 text-4xl font-bold tracking-tight text-black">
      {{ details.newValue }} {{ details.unit }}
    </h5>
    <div class="flex">
      <p :class="details.valueColor" class="mb-3 me-3 font-bold">
        {{ details.value }}
      </p>
      <p class="mb-3 font-normal">{{ details.moving }}</p>
    </div>
    <p class="mb-3 font-normal text-gray-500 dark:text-gray-400">
      {{ details.info }}
    </p>
    <p></p>
  </div>
</template>

<style>
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>

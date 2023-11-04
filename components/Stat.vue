<template>
    <div>
        <div class="text-orange-500 font-bold text-6xl mb-4">{{ number }}</div>
        <div class="text-white uppercase font-semibold text-xl">{{ caption }}</div>
    </div>
</template>

<script setup lang="ts">
const props = defineProps({
  number: String,
  caption: String,
});
</script>
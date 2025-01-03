<template>
  <button
    class="bg-blue-500 text-white px-4 py-1 rounded-3xl hover:bg-blue-600"
  >
    {{ props.text }}
  </button>
</template>

<script setup lang="ts">
const props = defineProps<{
  text: string;
}>();
</script>

<script setup>
defineProps(["title", "type"]);
</script>
<template>
  <button
    v-bind:type="type"
    class="inline-flex items-center px-4 py-2 rounded-md font-semibold tracking-widest focus:outline-none focus:[#23a100] focus:shadow-outline-gray transition ease-in-out duration-150 bg-green-400 hover:bg-green-500 active:bg-bg-green-600 text-white"
  >
    {{ title }}
  </button>
</template>

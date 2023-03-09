<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const currentTime = ref(new Date().toLocaleTimeString());

const interval = setInterval(() => {
  currentTime.value = new Date().toLocaleTimeString();
}, 1000);

onMounted(() => {
  console.log("Clock mounted");
});

onUnmounted(() => {
  console.log("Clock unmounted");
  clearInterval(interval);
});
</script>
<template>
  <div>
    {{ currentTime }}
  </div>
</template>

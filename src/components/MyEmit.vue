<script setup>
import BaseButton from "@/components/BaseButton.vue";

defineEmits(["onPress"]);
</script>

<template>
  <div
    class="flex flex-col items-center bg-white border shadow-lg rounded-lg w-80 p-5 gap-10"
  >
    <h2 class="text-lg">Hello I am Emit</h2>
    <BaseButton
      @click="$emit('onPress', 'Muzamil')"
      title="Call"
      class="w-full flex items-center justify-center"
    />
  </div>
</template>

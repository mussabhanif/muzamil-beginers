<script setup>
const props = defineProps({
  title: String,
  icon: String,
});
const check = () => {
  alert(props?.title);
};
// defineProps(["title"]);
</script>

<template>
  <button
    class="bg-green-500 py-2 px-3 text-white rounded-lg hover:bg-green-600 flex items-center justify-center"
  >
    <span v-if="icon" class="material-symbols-outlined"> {{ icon }} </span>

    <span v-if="title"> {{ title }}</span>
    <span>
      <slot />
    </span>
  </button>
</template>

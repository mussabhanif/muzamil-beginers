<script setup>
import { reactive } from "vue";

const state = reactive({
  name: "Musab",
  email: "musab@example.com",
  mybool: true,
  myNum: 1234,
  myNull: null,
  myArr: [
    {
      name: "dashrat",
      emai: "dashrat@karimapps.com",
    },
  ],
  user: {
    name: "Muzamil",
    email: "Muzamil@g.com",
  },
});
const arr = [1, 87878, 3, 4, 5, "musab"];
</script>

<template>
  <div>{{ state.myArr[0]?.name }}</div>
</template>

<style scoped></style>

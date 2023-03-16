<script setup>
import { reactive } from "vue";
import BaseButton from "@/components/BaseButton.vue";
import MyEmit from "@/components/MyEmit.vue";
import { RouterView } from "vue-router";

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
const callEmit = (name) => {
  alert("Hi i am emit. you are " + name);
};
const ClickMe = (id) => {
  alert(id + "clicked");
};
</script>

<template>
  <RouterView />
</template>

<style scoped></style>

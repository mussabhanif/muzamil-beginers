<script setup>
import BaseButton from "@/components/BaseButton.vue";
import BaseCard from "@/components/BaseCard.vue";
import BaseLayout from "@/components/layout/BaseLayout.vue";
import Clock from "./Clock.vue";
import { ref } from "vue";

const name = ref("");
const check = () => {
  console.log(name.value);
}
</script>

<template>
  <BaseLayout>
    <!-- temp:header -->
    <template v-slot:header>
      <BaseButton title="Logout" icon="logout" />
    </template>
    <!-- content -->
    <!-- <Clock /> -->
    <div class="flex flex-col gap-4 w-screen items-center">
      <div>
        <label for="name">Name</label>
        <input
          type="text"
          id="name"
          placeholder="Name"
          v-model="name"
          class="block w-80 flex-1 rounded-md border-0 py-1.5 px-2 text-gray-900 ring-1 ring-inset focus:outline-none ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"
        />
      </div>
      {{ name }}
      <BaseButton title="Submit" v-on:click="check"/>
    </div>

    <!--footer -->
    <!-- <template v-slot:footer>
      <div class="bg-green-500 py-2">
        <h3 class="text-3xl">Hi i am footer</h3>
      </div>
    </template> -->
  </BaseLayout>
</template>

<style scoped></style>

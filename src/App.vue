<script setup>
import BaseButton from "@/components/BaseButton.vue";
import BaseCard from "@/components/BaseCard.vue";
import BaseLayout from "@/components/layout/BaseLayout.vue";
</script>

<template>
  <BaseLayout>
    <!-- temp:header -->
    <template v-slot:header>
      <BaseButton title="Logout" icon="logout" />
    </template>

    <!--footer -->
    <template v-slot:footer>
      <div class="bg-green-500 py-2">
        <h3 class="text-3xl">Hi i am footer</h3>
      </div>
    </template>
  </BaseLayout>
</template>

<style scoped></style>

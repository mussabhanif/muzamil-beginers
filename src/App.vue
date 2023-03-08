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
    <!-- content -->
    <div class="flex flex-col gap-4">
      <h3 class="text-3xl">
        This is baselayout with named slots. this is our main content
      </h3>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis itaque debitis
        corporis delectus aliquid! Enim eaque labore distinctio consequatur quibusdam
        molestias officiis laboriosam vitae omnis ea aut asperiores, inventore beatae.
      </p>
    </div>
    <!--footer -->
    <template v-slot:footer>
      <div class="bg-green-500 py-2">
        <h3 class="text-3xl">Hi i am footer</h3>
      </div>
    </template>
  </BaseLayout>
</template>

<style scoped></style>

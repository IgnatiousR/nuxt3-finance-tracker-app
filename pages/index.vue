<template>
  <section class="flex items-center justify-between mb-10">
    <h1 class="text-4xl font-extrabold">Summary</h1>
    <div>
      <USelectMenu
        v-model="selectedView"
        :items="transactionViewOptions"
        class="w-32"
      />
    </div>
  </section>
</template>

<script setup>
import { transactionViewOptions } from "~/constants";
const selectedView = ref("Yearly");
</script>

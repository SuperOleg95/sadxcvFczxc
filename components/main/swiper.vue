<script setup lang="ts">
import { UButton } from "#components";

const items = [
  { color: "red", description: "loren ipsum" },
  { color: "green", description: "loren ipsum" },
  { color: "orange", description: "loren ipsum" },
  { color: "lime", description: "loren ipsum" },
  { color: "teal", description: "loren ipsum" },
  { color: "violet", description: "loren ipsum" },
  { color: "fuchsia", description: "loren ipsum" },
  { color: "gray", description: "loren ipsum" },
];
</script>

<template>
  <UCarousel
    v-slot="{ item }"
    :items="items"
    :ui="{ item: 'basis-full' }"
    class="rounded-lg !mt-0"
    arrows
    indicators
  >
    <div :class="`bg-${item.color}-500 w-full h-[580px] relative`">
      <div class="absolute left-[7%] top-[50%] space-y-2">
        <h1 class="text-2xl font-bold">Corporate webpage 2025</h1>
        <div class="h-1 w-20 bg-black"></div>
        <h5>
          New opportunities, income, resilience, projects...<br />
          Our web engineer look ahead to what 2025 will bring
        </h5>
        <UButton size="xl">Learn more</UButton>
      </div>
    </div>
  </UCarousel>
</template>

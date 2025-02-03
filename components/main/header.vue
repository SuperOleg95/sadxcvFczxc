<script setup lang="ts">
const links = [
  {
    label: "Software",
    icon: "i-heroicons-code-bracket",
    to: "#",
  },
  {
    label: "Engineering",
    icon: "i-heroicons-cog-8-tooth",
    to: "#",
  },
  {
    label: "Products",
    icon: "i-heroicons-sparkles",
    to: "#",
  },
  {
    label: "Company",
    icon: "i-heroicons-briefcase",
    to: "#",
  },
  {
    label: "Career",
    icon: "i-heroicons-presentation-chart-line",
    to: "#",
  },
];
</script>

<template>
  <MainContainer>
    <div class="flex justify-between">
      <div class="flex">
        <NuxtImg src="/logo.png" class="object-contain h-10" />
        <TypographyHeadline content="Schleißheimer" size="lg" />
      </div>

      <MainMegamenu />

      <div class="space-x-4">
        <CommonColorThemeSelector />
        <Icon name="mdi:earth" class="h-8 w-8"></Icon>
        <UIcon name="i-heroicons-magnifying-glass" class="h-8 w-8"></UIcon>
      </div>
    </div>
  </MainContainer>
</template>

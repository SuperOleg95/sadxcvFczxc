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
        <UIcon name="i-heroicons-globe-europe-africa" class="h-8 w-8"></UIcon>
        <UIcon name="i-heroicons-magnifying-glass" class="h-8 w-8"></UIcon>
      </div>
    </div>
  </MainContainer>
</template>

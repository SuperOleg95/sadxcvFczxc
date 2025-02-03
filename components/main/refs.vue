<script setup lang="ts">
import "~/assets/css/main.css";

definePageMeta({
  layout: "custom",
});

let logos = [
  {
    id: "conti",
    image: "/main/conti.jpg",
  },
  {
    id: "bender",
    image: "/main/bender.jpg",
  },
  {
    id: "kuster",
    image: "/main/kuster.jpg",
  },
  {
    id: "fresenius",
    image: "/main/fresenius.jpg",
  },
];
</script>

<template>
  <MainContainer>
    <div class="ps-4">
      <TypographyTitle>Our partners</TypographyTitle>
      <TypographyHeadline content="Trusted by many" size="lg" />
    </div>
    <div class="flow-root mt-8 lg:mt-10">
      <div
        v-if="logos && logos.length > 0"
        class="grid gap-4 md:grid-cols-4 md:gap-8"
      >
        <div
          v-for="(logo, fileIdx) in logos"
          :key="logo.id"
          v-motion
          :initial="{
            opacity: 0,
            y: 150,
          }"
          :visibleOnce="{
            opacity: 1,
            y: 0,
          }"
          :delay="250 + 200 * fileIdx"
          class="flex items-center justify-center"
        >
          <NuxtImg class="h-32" :src="logo.image" />
        </div>
      </div>
    </div>
  </MainContainer>
</template>

<template>
  <div class="bg-gray-200 min-h-screen">
    <NuxtPage class="dk-container dir bg-white mx-auto pb-24" />
    <div class="dk-menu sticky bottom-0 left-0 bg-white w-full z-50 mx-auto">
      salam
    </div>
  </div>
</template>
<script setup>
useHead(() => ({
  title: "Digikala USED",
  link: [
    {
      href: "https://fonts.cdnfonts.com/css/iranyekan",
      rel: "stylesheet",
      fetchpriority: "high",
      crossorigin: "anonymous",
    },
  ],
}));
</script>
<style>
.dk-container {
  min-width: 480px;
  width: 480px;
  min-height: calc(100vh - 112px);
  direction: rtl;
  font-family: "IRANYekan", sans-serif;
  font-display: swap;
}
.dk-menu {
  min-width: 480px;
  width: 480px;
  box-shadow: 0px -2px 2px 0px rgba(0, 0, 0, 0.1);
}
</style>

<template>
  <div class="bg-gray-200 min-h-screen dk-warpper">
    <NuxtPage class="dk-container dir bg-white mx-auto pb-24" />
    <BaseMenu />
  </div>
</template>
<script setup>
useHead(() => ({
  title: "دیجی‌کالا - خرید و فروش تلفن همراه کارکرده سریع، مطمئن، به‌صرفه",
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
}
.dk-warpper {
  direction: rtl;
  font-family: "IRANYekan", sans-serif;
  font-display: swap;
}
</style>

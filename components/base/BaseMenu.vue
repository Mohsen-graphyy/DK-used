<template>
  <div
    class="dk-menu grid grid-cols-3 sticky bottom-0 left-0 bg-white w-full z-50 mx-auto">
    <NuxtLink
      v-for="menuItem in menuItems"
      :key="menuItem.id"
      class="p-2 flex flex-col justify-center items-center gap-2"
      :to="{ name: menuItem.routeName }">
      <UIcon
        class="w-7 h-7"
        :class="
          $route.name === menuItem.routeName ? 'text-red-500' : 'text-gray-500'
        "
        :name="menuItem.icon" />
      <p class="font-light text-sm">{{ menuItem.lable }}</p>
    </NuxtLink>
  </div>
</template>

<script setup>
const menuItems = [
  { id: 1, icon: "i-heroicons-home", lable: "خانه", routeName: "home" },
  {
    id: 2,
    icon: "i-heroicons-building-storefront",
    lable: "فروشگاه",
    routeName: "shop",
  },
  {
    id: 3,
    icon: "i-heroicons-user",
    lable: "حساب کاربری",
    routeName: "profile",
  },
];
</script>

<style scoped>
.dk-menu {
  min-width: 480px;
  width: 480px;
  box-shadow: 0px -2px 2px 0px rgba(0, 0, 0, 0.1);
}
</style>

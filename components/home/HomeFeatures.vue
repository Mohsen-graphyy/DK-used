<template>
  <img
    src="/images/poster.jpg"
    width="480px"
    height="343px"
    alt="campain-poster" />
  <div class="p-3 mt-2 mb-3 flex justify-between items-center">
    <img src="/images/buyBtn.png" width="210px" height="100px" alt="buy" />
    <img src="/images/sellBtn.png" width="210px" height="100px" alt="sell" />
  </div>
  <div class="grid grid-cols-4 items-center mx-3 justify-center">
    <div
      v-for="feature in features"
      :key="feature.src"
      class="flex justify-center items-center flex-col">
      <img :src="feature.src" width="52px" height="52px" :alt="feature.label" />
      <p class="text-xs mt-2 font-light">{{ feature.label }}</p>
    </div>
  </div>
</template>

<script setup lang="ts">
const features = [
  {
    src: "/images/homeNewPrice2.svg",
    label: "بهترین قیمت",
  },
  {
    src: "data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUiIGhlaWdodD0iNDUiIHZpZXdCb3g9IjAgMCA0NSA0NSIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHJlY3Qgd2lkdGg9IjQ0LjY1MTIiIGhlaWdodD0iNDQuNjUxMiIgcng9IjEyIiBmaWxsPSIjRkZFREVGIi8+CjxwYXRoIGQ9Ik05LjA3NjgyIDE1LjEyMDZDOS4wMzAyNiAxNC4yMzYgOS41MTc4OCAxMy40MDk0IDEwLjMxNDcgMTMuMDIyM0wxOS4zNDE2IDguNjM2ODhDMjAuMTY5MyA4LjIzNDc2IDIxLjEzNTggOC4yMzQ3NiAyMS45NjM1IDguNjM2ODhMMzAuOTkwNCAxMy4wMjIzQzMxLjc4NzIgMTMuNDA5NCAzMi4yNzQ4IDE0LjIzNiAzMi4yMjgzIDE1LjEyMDZMMzEuOTQ3OCAyMC40NDk0QzMxLjU5MzQgMjcuMTgyNCAyNy41ODczIDMzLjE4MzQgMjEuNTA0NyAzNi4wOTI0QzIwLjk2NTggMzYuMzUwMiAyMC4zMzkyIDM2LjM1MDIgMTkuODAwMyAzNi4wOTI0QzEzLjcxNzggMzMuMTgzNCA5LjcxMTY1IDI3LjE4MjQgOS4zNTcyOCAyMC40NDk0TDkuMDc2ODIgMTUuMTIwNloiIGZpbGw9IiNERjM2NEIiLz4KPHBhdGggZD0iTTE2LjE1MjYgMjEuNUwxOS42NTI2IDI1TDI1LjY1MjYgMTkiIHN0cm9rZT0id2hpdGUiIHN0cm9rZS13aWR0aD0iMiIvPgo8Y2lyY2xlIG9wYWNpdHk9IjAuNSIgY3g9IjI5LjE1MjYiIGN5PSIzMSIgcj0iNyIgZmlsbD0iI0I3MjYzOCIvPgo8L3N2Zz4K",
    label: "امن و معتبر",
  },
  {
    src: "/images/homeNewFast2.svg",
    label: "سریع و آسوده",
  },
  {
    src: "data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUiIGhlaWdodD0iNDUiIHZpZXdCb3g9IjAgMCA0NSA0NSIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHJlY3Qgd2lkdGg9IjQ0LjY1MTIiIGhlaWdodD0iNDQuNjUxMiIgcng9IjEyIiBmaWxsPSIjRkZFREVGIi8+CjxyZWN0IHg9IjEwLjUiIHk9IjEyIiB3aWR0aD0iMjMiIGhlaWdodD0iMjMiIHJ4PSIyIiBmaWxsPSIjRDgzNTRBIiBzdHJva2U9IiNEODM1NEEiIHN0cm9rZS13aWR0aD0iMiIvPgo8cGF0aCBkPSJNMTUuNSAxNVY5IiBzdHJva2U9IiNEODM1NEEiIHN0cm9rZS13aWR0aD0iMiIvPgo8cGF0aCBkPSJNMjguNSAxNVY5IiBzdHJva2U9IiNEODM1NEEiIHN0cm9rZS13aWR0aD0iMiIvPgo8Y2lyY2xlIG9wYWNpdHk9IjAuNSIgY3g9IjMyIiBjeT0iMzEuNSIgcj0iNy41IiBmaWxsPSIjQjcyNjM4Ii8+CjxwYXRoIGQ9Ik05LjUgMTlIMzQuNSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIi8+CjxwYXRoIGQ9Ik0xNCAyNS40TDE2LjcwODIgMjguNTM0OUMxNi45MTU1IDI4Ljc3NDggMTcuMjkwOSAyOC43NjM3IDE3LjQ4MzYgMjguNTEyTDI0IDIwIiBzdHJva2U9IndoaXRlIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJzcXVhcmUiLz4KPC9zdmc+Cg==",
    label: "گارانتی دیجی‌کالا",
  },
];
</script>

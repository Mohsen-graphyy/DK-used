<template>
  <div
    class="border border-solid border-gray-200 p-3 rounded-lg max-w-full min-w-[334px] h-[224px]">
    <p class="font-semibold text-xs my-1">{{ testimonial.title }}</p>
    <div
      class="flex items-center justify-start gap-2 mt-4"
      :class="testimonial.isPrefer ? 'text-green-600' : 'text-red-600'">
      <UIcon
        class="w-4 h-4"
        :name="
          testimonial.isPrefer
            ? 'i-heroicons-hand-thumb-up'
            : 'i-heroicons-hand-thumb-down'
        " />
      <p class="text-xs">
        پیشنهاد {{ testimonial.isPrefer ? "می‌کنم" : "نمی‌کنم" }}
      </p>
    </div>
    <p class="text-xs mt-4">
      {{ testimonial.comment }}
    </p>
    <p class="list-item text-xs text-gray-500 mt-4 list-inside">
      {{ testimonial.author }}
    </p>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  testimonial: {
    id: number;
    title: string;
    isPrefer: boolean;
    comment: string;
    author: string;
  };
}>();
</script>

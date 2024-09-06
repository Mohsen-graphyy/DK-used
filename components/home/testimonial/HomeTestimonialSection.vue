<template>
  <div
    class="overflow-x-scroll w-full flex flex-nowrap items-center gap-4 mt-8 p-3">
    <HomeTestimonial
      v-for="testimonial in testimonials"
      :key="testimonial.id"
      :testimonial="testimonial" />
  </div>
</template>

<script setup lang="ts">
const testimonials = [
  {
    id: 1,
    title: "گارانتی دیجیکالا",
    isPrefer: true,
    comment: `تقریبا یکسالی بود که فکر خرید گوشی بودم ولی قیمت هاخیلی فاجعه بود. تصمیم گرفتم گوشی دست دوم بخرم ولی نگران بودم که گوشی ایراددار بهم بدن و بعدشم دستم به جایی بند نباشه. الان که گوشی گارانتی شده خریدم واقعا خیالم راحته. `,
    author: "Parmida Mirzaei",
  },
  {
    id: 2,
    title: "قیمت مناسب",
    isPrefer: false,
    comment: `اولش که اطلاعات رو وارد کردم باورم نشد که 36 تومن گوشیمو میخرن. من یک روز تمام از هر مغازه‌ای پرسیدم 30 تا 32 تومن بیشتر بر نمی‌داشتن. بدون هیچ زحمت و دردسری اومدن گوشیو ازم تحویل گرفتن و کارشناسیش کردنو چون واقعا گوشیم در حد نو بود عینا همون مبلغ رو بهم پرداخت کردن `,
    author: "Soheil Taghavi",
  },
  {
    id: 3,
    title: "کارشناسی رایگان ",
    isPrefer: true,
    comment: `بدون اینکه هزینه ای پرداخت کنم گوشیموکارشناش کردن و با قیمت منصفانه ای توافق کردم بفروشم و کمکم کردن با همون قیمت بتونم یه گوشی مدل بالا کارکرده با 3 ماه گارانتی بخرم `,
    author: "Soheila Alemi",
  },
  {
    id: 4,
    title: "مهلت ۷ روزه ",
    isPrefer: true,
    comment: `اینکه 7 روز مهلت تست دادن خیال منو از خرید راحت کرد که خوشبختانه مشکلی هم پیش نیومد. گوشی عینا مطابق توضیحاتش بود `,
    author: "Hossein Sharify",
  },
];
</script>

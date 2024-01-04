<script setup>
defineProps({
  imageUrl: String,
  productName: String,
  productPrice: Number
})
</script>

<template>
  <div class="gap-3 flex items-end w-full border rounded-2xl p-5">
    <div class="flex gap-5 items-center">
      <img :src="imageUrl" alt="image" class="w-20 h-20 object-contain" />
      <div class="">
        <span class="text-sm font-normal line-clamp-2">{{ productName }}</span>
        <span class="text-sm font-bold">{{ productPrice }} rub.</span>
      </div>
    </div>
    <img src="/close.svg" alt="icon" class="cursor-pointer" />
  </div>
</template>

<script setup>
defineProps({
  imageUrl: String,
  title: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  addToFavorite: Function,
  addToCart: Function
})
</script>

<template>
  <div
    class="bg-white rounded-3xl border w-fit p-7 flex flex-col gap-3.5 cursor-pointer hover:-translate-y-2 hover:shadow-xl transition"
  >
    <div class="relative">
      <img
        :src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
        alt="icon"
        class="absolute t-2.5 w-8 h-8"
        @click="addToFavorite"
      />
      <img :src="imageUrl" alt="image" class="w-full max-w-32" />
    </div>
    <h1 class="line-clamp-2 max-w-36 text-sm">{{ title }}</h1>
    <div class="flex justify-between items-center">
      <div class="flex flex-col items-start">
        <span class="text-xs text-gray-500 font-medium">Цена:</span>
        <span class="font-bold">{{ price }}</span>
      </div>
      <img :src="isAdded ? '/checked.svg' : '/plus.svg'" alt="icon" @click="addToFavorite" />
    </div>
  </div>
</template>

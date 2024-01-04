<script setup>
import CartItem from './CartItem.vue'
</script>

<template>
  <main class="relative cart-scrollbar flex flex-col gap-6 h-2/3 overflow-auto pr-1 flex-grow">
    <CartItem
      :image-url="'/sneakers/sneakers-2.jpg'"
      :product-name="'something something something something something something'"
      :product-price="789500"
    />
  </main>
</template>

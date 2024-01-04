<script setup>
import Card from '../card/Card.vue'

const addToFavorite = () => {
  console.log('works');
}

const addToCart = () => {}
</script>

<template>
  <div class="grid grid-cols-3 gap-10">
    <Card
      :image-url="'/sneakers/sneakers-1.jpg'"
      :title="'ab provident corrupti, et saepe expedita quaerat! Voluptas, natus?'"
      :price="5000"
      :is-favorite="false"
      :is-added="false"
      :add-to-favorite="addToFavorite"
      :add-to-cart="addToCart"
    />
  </div>
</template>

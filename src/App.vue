<script setup>
import Header from './components/Header.vue'
import Card from './components/Card.vue'
</script>

<template>
  <div class="wrapper w-4/5 m-auto px-14 bg-white rounded-xl shadow-xl mt-14">
    <Header />

    <h1 class="text-2xl font-bold my-10">Все кроссовки</h1>

    <div class="grid grid-cols-3 gap-10">
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
    </div>
  </div>
</template>

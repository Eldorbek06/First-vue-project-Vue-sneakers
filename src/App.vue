<script setup>
import Header from './components/Header.vue'
import CardList from './components/card/CardList.vue'
import Drawer from './components/drawer/Drawer.vue'
</script>

<template>
  <div class="wrapper w-4/5 m-auto px-14 bg-white rounded-xl shadow-xl my-14 pb-10">
    <Header />

    <h1 class="text-2xl font-bold my-10">Все кроссовки</h1>

    <CardList />

    <Drawer />
  </div>
</template>

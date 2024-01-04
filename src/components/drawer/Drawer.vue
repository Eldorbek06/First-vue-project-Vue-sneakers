<script setup>
import CartItemList from '../cart/CartItemList.vue'
import DrawerHeader from './DrawerHeader.vue'
import DrawerFooter from './DrawerFooter.vue'

const toggleDrawer = (isOpen) => {
  const drawerEl = document.querySelector('#drawer')

  if (isOpen) {
    drawerEl.classList.add('hidden')
  } else {
    drawerEl.classList.remove('hidden')
  }
  console.log(drawerEl)
}
</script>

<template>
  <aside id="drawer" class="transition fixed top-0 left-0 w-full h-full bg-black/50">
    <div @click="toggleDrawer(true)" class="absolute z-10 top-0 left-0 w-full h-full"></div>
    <div
      class="absolute z-20 top-0 right-0 bottom-0 w-1/3 bg-white p-7 text-2xl font-bold flex flex-col"
    >
      <DrawerHeader />

      <CartItemList />

      <DrawerFooter />
    </div>
  </aside>
</template>

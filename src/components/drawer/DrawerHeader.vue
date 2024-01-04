<script setup>
const toggleDrawer = (isOpen) => {
  const drawerEl = document.querySelector('#drawer')

  if (isOpen) {
    drawerEl.classList.add = 'hidden'
  } else {
    drawerEl.classList.remove = 'hidden'
  }
  console.log(drawerEl)
}
</script>

<template>
   <header class="flex gap-4 mb-7">
        <img
          @click="toggleDrawer(true)"
          src="/arrow-next.svg"
          alt="icon"
          class="cursor-pointer invert opacity-50 hover:opacity-100 transition rotate-180 hover:-translate-x-1"
        />
        <h1 class="">Корзина</h1>
      </header>
</template>
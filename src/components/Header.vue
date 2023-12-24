<template>
  <header class="header py-11 flex justify-between items-center border-b">
    <div class="header__left flex gap-4 items-center">
      <img src="/logo.png" alt="logo" class="header__logo w-10 h-10" />
      <div class="header__text">
        <h1 class="header__title text-xl font-bold">VUE SNEAKERS</h1>
        <span class="header__sub-title text-sm text-gray-400">Best market of sneakers</span>
      </div>
    </div>
    <ul class="header__right flex gap-8 items-center">
      <li
        class="header__item flex items-center gap-2 text-gray-500 hover:text-black cursor-pointer"
      >
        <img src="/cart.svg" alt="icon" class="header__item-icon w-[18px] h-[18px]" />
        <span class="header__item-text text-sm font-semibold">1205 rub.</span>
      </li>
      <li
        class="header__item flex items-center gap-2 text-gray-500 hover:text-black cursor-pointer"
      >
        <img src="/heart.svg" alt="icon" class="header__item-icon w-[18px] h-[18px]" />
        <span class="header__item-text text-sm">favorites</span>
      </li>
      <li
        class="header__item flex items-center gap-2 text-gray-500 hover:text-black cursor-pointer"
      >
        <img src="/profile.svg" alt="icon" class="header__item-icon w-[18px] h-[18px]" />
        <span class="header__item-text text-sm">profile</span>
      </li>
    </ul>
  </header>
</template>

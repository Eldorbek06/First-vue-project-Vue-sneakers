<template>
  <footer class="w-full mt-4">
    <div class="font-normal text-base mb-6 flex flex-col gap-5">
      <p class="border-b flex justify-between">
        <span>Total:</span>
        <b>21 498 rub.</b>
      </p>
      <p class="border-b flex justify-between">
        <span>Tax 5%:</span>
        <b>1074 rub.</b>
      </p>
    </div>
    <button
      type="submit"
      disabled
      class="disabled:bg-gray-500 bg-lime-500 hover:bg-lime-600 transition text-white text-base font-semibold w-full rounded-2xl py-4 text-center relative"
    >
      <span>Checkout</span>
      <img class="absolute right-8 top-1/2 -translate-y-1/2" src="/arrow-next.svg" alt="icon" />
    </button>
  </footer>
</template>
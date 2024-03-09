<script setup>
const emit = defineEmits(['openDrawer'])
</script>

<template>
  <div class="bg-white w-screen h-20 rounded m-auto">
    <div class="flex justify-between px-8 pt-2">
      <div class="flex items-center">
        <img class="mr-5 cursor-pointer w-16" src="/public/images/real-estate.png" alt="" />
        <div>
          <h2 class="text-xl">Real</h2>
          <p class="text-slate-500">estate</p>
        </div>
        <div>
          <button
            @click="() => emit('openDrawer')"
            class="rounded-xl ease-in duration-300 w-24 h-16 hover:shadow-xl ml-10 mr-5"
          >
            Покупка
          </button>
          <button class="rounded-xl ease-in duration-300 w-24 h-16 hover:shadow-xl mr-5">
            Аренда
          </button>
          <button class="rounded-xl ease-in duration-300 w-24 h-16 hover:shadow-xl mr-5">
            Ипотека
          </button>
        </div>
      </div>
      <ul class="flex items-center">
        <li class="mr-5">
          <img
            class="opacity-40 ease-in duration-200 hover:opacity-100 cursor-pointer right w-12 h-12"
            src="/public/images/heart.png"
            alt=""
          />
        </li>
        <li>
          <button class="rounded-xl ease-in duration-300 w-24 h-16 hover:shadow-xl">Войти</button>
        </li>
      </ul>
    </div>
  </div>
</template>

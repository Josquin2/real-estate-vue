<script setup>
import rentList from './rent-list.vue'
import { inject } from 'vue'
const { closeDrawer } = inject('cardActions')
</script>
<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black opacity-60"></div>
  <div class="rounded-xl mx-auto bg-white top-0 left-32 h-2/3 w-4/5 fixed mt-20 p-8 flexbox">
    <div class="items-center flex">
      <img
        @click="() => closeDrawer()"
        class="opacity-30 w-10 h-10 rotate-90 cursor-pointer ease-in duration-200 hover:opacity-100"
        src="/public/images/arrow.png"
        alt=""
      />
      <h2 class="text-4xl pl-8">Аренда</h2>
    </div>
    <rentList />
  </div>
</template>

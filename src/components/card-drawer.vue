<script setup>
defineProps({
  imageUrl: String,
  title: String,
  otherInformation: String
})
</script>

<template>
  <div
    class="bg-white w-80 h-40 m-4 cursor-pointer border rounded-xl hover:shadow-xl ease-in duration-200"
  >
    <img class="ml-4 mt-6" :src="imageUrl" alt="" />
    <div class="ml-6 mt-3">
      <b>{{ title }}</b>
      <p class="opacity-30">{{ otherInformation }}</p>
    </div>
  </div>
</template>

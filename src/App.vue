<script setup>
import { provide, ref } from 'vue'

import Header from './components/header.vue'
import buyDrawer from './components/buy-drawer.vue'
import Hello from './components/hello-page.vue'
import rentList from './components/rent/rent-drawer.vue'

const drawerOpen = ref(false)

const closeDrawer = () => {
  drawerOpen.value = false
}

const openDrawer = () => {
  drawerOpen.value = true
}

provide('cardActions', {
  closeDrawer,
  openDrawer
})
</script>

<template>
  <Header @open-drawer="openDrawer" />
  <buyDrawer v-if="drawerOpen" />
  <!-- <Hello /> -->
  <!-- <rentList /> -->
</template>

<style>
body {
  background-color: rgb(235, 235, 235);
}
</style>

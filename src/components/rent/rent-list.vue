<script setup>
import Card from '../card-drawer.vue'
</script>

<template>
  <div class="grid grid-cols-3">
    <Card image-url="/public/images/house.png" title="Дом" other-information="Всего домов: 123" />
    <Card
      image-url="/public/images/apartment.png"
      title="Квартира"
      other-information="Всего квартир: 123"
    />
    <Card
      image-url="/public/images/new-apart.png"
      title="Новостройки"
      other-information="Всего новостроек: 213"
    />
    <Card
      image-url="/public/images/townhouse.png"
      title="Таунхаус"
      other-information="Всего таунхаусов: 123"
    />
  </div>
</template>

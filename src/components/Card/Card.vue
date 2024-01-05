<script setup>

  defineProps({
    item: Number,
    imageURL: String,
    price: Number,
    name: String,
    infoWeight: String,
  })

</script>

<template>
  <div class="menu__card">
    <img class="menu__card-img" :src="imageURL" alt="Sushi" />
    <h3 class="menu__card-name" style="padding-top: 20px; padding-bottom: 78px">
      {{ name }}
    </h3>
    <p class="menu__card-desc">{{ infoWeight }}</p>
    <div class="menu__card-price">
      <p class="menu__card-text">{{ price }} UAH</p>
      <button class="menu__card-btn">Хочу!</button>
    </div>
  </div>
</template>

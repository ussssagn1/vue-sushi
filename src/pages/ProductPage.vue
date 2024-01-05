<script setup>
import Card from '@/components/Card/Card.vue'
import { reactive, onMounted, ref, watch } from 'vue'
import axios from 'axios'

const product = ref([])
const filtered = reactive({
  sortBy: 'title',
  searchQuery: ''
})

const fetchItems = async () => {
  try {
    const params = {
      sortBy: filtered.sortBy
    }
    if(filtered.searchQuery) {
      params.title = `*${filtered.searchQuery}`
    }
    const { data } = await axios.get('https://81700eb106e9881c.mokky.dev/items', {
      params
    })
    product.value = data
  } catch (e) {
    console.log(`Ошибка при полученни данных: ${e}`)
  }
}

const onChangeSelect = (e) => {
  filtered.sortBy = e.target.value
  console.log(filtered.sortBy)
}

onMounted(fetchItems)
watch(filtered, fetchItems)
</script>

<template>
  <section class="menu">
    <div class="container-fluid">
      <div class="menu__up">
        <h1 class="menu__title">
          <img src="/Сеты.svg" alt="" />
          <span class="menu__title-text">Cеты</span>
        </h1>
        <div class="menu__select">
          <label for="menu__select" class="label">Сортировка: </label>
          <select @change="onChangeSelect" id="menu__select" class="menu__select-list">
            <option value="all">По умолчанию</option>
            <option value="name">Название</option>
            <option value="-price">Сначала дороже</option>
            <option value="price">Сначала дешевле</option>
          </select>
        </div>
      </div>

      <div class="menu__cards" v-auto-animate>
        <Card
          v-for="item in product"
          :key="item.id"
          :item="item.id"
          :imageURL="item.imageURL"
          :name="item.name"
          :infoWeight="item.infoWeight"
          :price="item.price"
        />
      </div>
    </div>
  </section>
</template>

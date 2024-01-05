<script setup>
import Swiper from 'swiper'
import { Navigation, Pagination } from 'swiper/modules'
import 'swiper/css/navigation'
import 'swiper/css/pagination'
import 'swiper/css'
import { onMounted } from 'vue'
import NavItem from './components/Navigation/NavItem.vue'
import CartItem from './components/Cart/CartItem.vue'
import HeaderBlock from './components/Main/HeaderBlock.vue'
import FooterBlock from './components/Main/FooterBlock.vue'
import ProductPage from './pages/ProductPage.vue'

onMounted(() => {
  new Swiper('.swiper', {
    modules: [Navigation, Pagination],
    // Optional parameters
    loop: true,

    pagination: {
      el: '.swiper-pagination'
    }
  }),
    new Swiper('.swipeNew', {
      // Optional parameters
      loop: false,
      slidesPerView: 3,
      spaceBetween: 30,

      // Navigation arrows
      navigation: {
        nextEl: '.cardNext',
        prevEl: '.cardPrev'
      }
    })
})
</script>

<template>
  <div class="container">
    <div class="wrapper">
      <NavItem />

      <div class="mainCont">
        <HeaderBlock />
        <main class="main">
          <ProductPage />
        </main>
        <FooterBlock />
      </div>

      <CartItem />
    </div>
  </div>
</template>

<style scoped></style>

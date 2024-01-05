<script setup></script>

<template>
  <aside>
    <div class="cartMenu">
      <div v-if="true" class="cartClose">
        <div class="cart">
          <div class="cart__text">
            <h3 class="cart__title">Ваша корзина пуста.</h3>
            <p class="cart__desc">Добавьте же скорее что-нибудь!</p>
          </div>
          <div class="cart__free">Бесплатная доставка от 800 UAH</div>
        </div>
        <div class="cartMap">
          <iframe
            class="CartMap__img"
            src="https://www.google.com/maps/embed?pb=!1m10!1m8!1m3!1d20309.075323923767!2d30.4721233!3d50.4851493!3m2!1i1024!2i768!4f13.1!5e0!3m2!1sru!2sua!4v1704228820860!5m2!1sru!2sua"
            width="290"
            height="200"
            style="border: 0"
            allowfullscreen=""
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
          <h3 class="cart__title">Укажите адрес</h3>
          <p class="cart__desc">И узнайте время доставки</p>
        </div>
      </div>

      <div v-else class="cartFull">
        <h2 class="cartFull__title">Корзина</h2>
        <div class="cartFull__product">
          <img class="cartFull__product-img" src="/cart/sushi.png" alt="sushi" />
          <div class="cartFull__info">
            <h5 class="cartFull__info-title">Самая большая Фи...</h5>
            <div class="cartFull__info-count">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="12"
                height="2"
                viewBox="0 0 12 2"
                fill="none"
              >
                <path d="M1 1L11 1" stroke="#111111" stroke-width="2" stroke-linecap="round" />
              </svg>
              <span>10</span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="20"
                height="20"
                viewBox="0 0 20 20"
                fill="none"
              >
                <ellipse
                  cx="10.3602"
                  cy="10.2589"
                  rx="9.64029"
                  ry="9.64029"
                  transform="rotate(90 10.3602 10.2589)"
                  fill="#F46D40"
                />
                <path
                  d="M10.3604 4.95679V15.0791"
                  stroke="#F2F2F2"
                  stroke-width="2"
                  stroke-linecap="round"
                />
                <path
                  d="M5.54004 9.77698L15.6623 9.77698"
                  stroke="#F2F2F2"
                  stroke-width="2"
                  stroke-linecap="round"
                />
              </svg>
              <span class="cartFull__info-price">170 UAH</span>
            </div>
          </div>
        </div>
        <div class="cartFull__orders">
          <span class="cardFull__orders-price">150 UAH</span>
          <button class="cartFull__orders-button">Офоримть заказ</button>
        </div>
      </div>
    </div>
  </aside>
</template>

<style></style>

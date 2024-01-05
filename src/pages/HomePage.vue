<script setup></script>

<template>
  <div class="home">
    <section class="advertising">
      <div class="container-fluid">
        <div class="swiper">
          <div class="swiper-wrapper">
            <div class="swiper-slide">
              <a href="" class="advertising-link">
                <img src="/advertising.png" alt="" class="advertising" />
              </a>
            </div>
            <div class="swiper-slide">
              <a href="" class="advertising-link">
                <img src="/advertising.png" alt="" class="advertising" />
              </a>
            </div>
            <div class="swiper-slide">
              <a href="" class="advertising-link">
                <img src="/advertising.png" alt="" class="advertising" />
              </a>
            </div>
            <div class="swiper-slide">
              <a href="" class="advertising-link">
                <img src="/advertising.png" alt="" class="advertising" />
              </a>
            </div>
            <div class="swiper-slide">
              <a href="" class="advertising-link">
                <img src="/advertising.png" alt="" class="advertising" />
              </a>
            </div>
          </div>
          <div class="swiper-pagination"></div>
        </div>
        <div class="advertising__cards">
          <div class="advertising__card">
            <img src="/cardsOthers/С лососем.png" alt="" class="advertising__card-img" />
            <p class="advertising__card-text">Чикен</p>
          </div>
          <div class="advertising__cards-two">
            <div class="advertising__card-two">
              <img
                src="/cardsOthers/С угрем.png"
                alt=""
                class="advertising__card-two-img"
              />
              <p class="advertising__card-two-text">С угрем</p>
            </div>
            <div class="advertising__card-two">
              <img
                src="/cardsOthers/Без мяса.png"
                alt=""
                class="advertising__card-two-img"
              />
              <p class="advertising__card-two-text">Корн дог</p>
            </div>
          </div>
          <div class="advertising__card">
            <img
              src="/cardsOthers/С филадельфией.png"
              alt=""
              class="advertising__card-img"
            />
            <p class="advertising__card-text">Пицца</p>
          </div>
          <div class="advertising__card">
            <img src="/cardsOthers/Акции.png" alt="" class="advertising__card-img" />
            <p class="advertising__card-text">Акции</p>
          </div>
        </div>
      </div>
    </section>
    <section class="popular">
      <div class="container-fluid">
        <span class="popular__text">Новинки</span>
        <span class="popular__text-active">Популярное</span>
        <div class="swipeNew">
          <div class="swiper-wrapper">
            <div class="swiper-slide">
              <div class="popular__card">
                <img class="popular__card-img" src="/newSushi/Salomon.png" alt="" />
                <h3 class="popular__card-name">Соломон сет</h3>
                <p class="popular__card-desc">1050 грамм, 30 кусочков</p>
                <div class="popular__card-price">
                  <p class="popular__card-text">1500 UAH</p>
                  <button class="popular__card-btn">Хочу!</button>
                </div>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="popular__card">
                <img class="popular__card-img" src="/newSushi/FIladelfia.png" alt="" />
                <h3 class="popular__card-name">Филадельфия и лосось сет</h3>
                <p class="popular__card-desc">1260 грамм, 36 кусочков</p>
                <div class="popular__card-price">
                  <p class="popular__card-text">1150 UAH</p>
                  <button class="popular__card-btn">Хочу!</button>
                </div>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="popular__card">
                <img class="popular__card-img" src="/newSushi/BigFiladelfia.png" alt="" />
                <h3 class="popular__card-name">Самая большая Филадельфия</h3>
                <p class="popular__card-desc">2050 грамм, 45 кусочков</p>
                <div class="popular__card-price">
                  <p class="popular__card-text">2100 UAH</p>
                  <button class="popular__card-btn">Хочу!</button>
                </div>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="popular__card">
                <img class="popular__card-img" src="/newSushi/Salomon.png" alt="" />
                <h3 class="popular__card-name">Соломон сет</h3>
                <p class="popular__card-desc">1050 грамм, 30 кусочков</p>
                <div class="popular__card-price">
                  <p class="popular__card-text">1500 UAH</p>
                  <button class="popular__card-btn">Хочу!</button>
                </div>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="popular__card">
                <img class="popular__card-img" src="/newSushi/FIladelfia.png" alt="" />
                <h3 class="popular__card-name">Филадельфия и лосось сет</h3>
                <p class="popular__card-desc">1260 грамм, 36 кусочков</p>
                <div class="popular__card-price">
                  <p class="popular__card-text">1150 UAH</p>
                  <button class="popular__card-btn">Хочу!</button>
                </div>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="popular__card">
                <img class="popular__card-img" src="/newSushi/BigFiladelfia.png" alt="" />
                <h3 class="popular__card-name">Самая большая Филадельфия</h3>
                <p class="popular__card-desc">2050 грамм, 45 кусочков</p>
                <div class="popular__card-price">
                  <p class="popular__card-text">2100 UAH</p>
                  <button class="popular__card-btn">Хочу!</button>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="cardNext">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="60"
            height="60"
            viewBox="0 0 60 60"
            fill="none"
          >
            <ellipse cx="30" cy="30" rx="30" ry="30" transform="rotate(90 30 30)" fill="#111111" />
            <path d="M23 15L36 28.5L23 42" stroke="#F2F2F2" stroke-linecap="round" />
          </svg>
        </div>
        <div class="cardPrev">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="60"
            height="60"
            viewBox="0 0 60 60"
            fill="none"
          >
            <ellipse cx="30" cy="30" rx="30" ry="30" transform="rotate(90 30 30)" fill="#111111" />
            <path d="M36 15L23 28.5L36 42" stroke="#F2F2F2" stroke-linecap="round" />
          </svg>
        </div>
      </div>
    </section>
  </div>
</template>

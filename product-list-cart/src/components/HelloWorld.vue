<template>
  <div class="container">
    <section class="product-list">
      <header class="product-list__header">
        <h1>Desserts</h1>
      </header>
      <article class="product-list__content">
        <div
          class="product-list__content-card"
          v-for="(info, index) in data"
          :key="index"
        >
          <img
            class="product-list__content-card-image"
            :src="info.image.desktop"
            alt=""
          />
          <button class="product-list__content-card-button">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="21"
              height="20"
              fill="none"
              viewBox="0 0 21 20"
            >
              <g fill="#C73B0F" clip-path="url(#a)">
                <path
                  d="M6.583 18.75a1.25 1.25 0 1 0 0-2.5 1.25 1.25 0 0 0 0 2.5ZM15.334 18.75a1.25 1.25 0 1 0 0-2.5 1.25 1.25 0 0 0 0 2.5ZM3.446 1.752a.625.625 0 0 0-.613-.502h-2.5V2.5h1.988l2.4 11.998a.625.625 0 0 0 .612.502h11.25v-1.25H5.847l-.5-2.5h11.238a.625.625 0 0 0 .61-.49l1.417-6.385h-1.28L16.083 10H5.096l-1.65-8.248Z"
                />
                <path
                  d="M11.584 3.75v-2.5h-1.25v2.5h-2.5V5h2.5v2.5h1.25V5h2.5V3.75h-2.5Z"
                />
              </g>
              <defs>
                <clipPath id="a">
                  <path fill="#fff" d="M.333 0h20v20h-20z" />
                </clipPath>
              </defs>
            </svg>
            Add to Cart
          </button>

          <footer class="product-list__content-card-footer">
            <div class="product-list__content-card-footer__text">
              <p>{{ info.category }}</p>
              <p>{{ info.name }}</p>
              <p>${{ info.price }}</p>
            </div>
          </footer>
        </div>
      </article>
    </section>
    <aside class="cart">
      <header class="cart__header">
        <h3>Your Cart (7)</h3>
      </header>
      <article class="cart__products">
        <ul class="cart__products-item" >
          <li class="cart__products-item__list">
            <span class="cart__products-item__name">Classic Tiramisu</span>
            <span class="cart__products-item__icon">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="10"
                height="20"
                fill="none"
                viewBox="0 0 10 10"
              >
                <path
                  fill="#CAAFA7"
                  d="M8.375 9.375 5 6 1.625 9.375l-1-1L4 5 .625 1.625l1-1L5 4 8.375.625l1 1L6 5l3.375 3.375-1 1Z"
                />
              </svg>
            </span>
            <div class="cart__products-item__quantity">
              <span class="cart__quantity__color"> 1x </span>
              <span class="cart__price__color"> @5.50 </span>
              <span class="cart__total__color"> $5.50 </span>
            </div>
          </li>
          <div class="divider"></div>
          <li class="cart__products-item__list">
            <span class="cart__products-item__name">Classic Tiramisu</span>
            <span class="cart__products-item__icon">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="10"
                height="20"
                fill="none"
                viewBox="0 0 10 10"
              >
                <path
                  fill="#CAAFA7"
                  d="M8.375 9.375 5 6 1.625 9.375l-1-1L4 5 .625 1.625l1-1L5 4 8.375.625l1 1L6 5l3.375 3.375-1 1Z"
                />
              </svg>
            </span>
            <div class="cart__products-item__quantity">
              <span class="cart__quantity__color"> 4x </span>
              <span class="cart__price__color"> @6.50 </span>
              <span class="cart__total__color"> $28.00 </span>
            </div>
          </li>
          <div class="divider"></div>

          <li class="cart__products-item__list">
            <span class="cart__products-item__name">Classic Tiramisu</span>
            <span class="cart__products-item__icon">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="10"
                height="20"
                fill="none"
                viewBox="0 0 10 10"
              >
                <path
                  fill="#CAAFA7"
                  d="M8.375 9.375 5 6 1.625 9.375l-1-1L4 5 .625 1.625l1-1L5 4 8.375.625l1 1L6 5l3.375 3.375-1 1Z"
                />
              </svg>
            </span>
            <div class="cart__products-item__quantity">
              <span class="cart__quantity__color"> 2x </span>
              <span class="cart__price__color"> @6.50 </span>
              <span class="cart__total__color"> $13.00 </span>
            </div>
          </li>
          <div class="divider"></div>
        </ul>
      </article>
      <footer
        class="cart__products-total"
       
      >
        <div
          class="cart__products-item_total"
          style="display: grid; grid-template-columns: auto auto"
        >
          <p>Order Total</p>
          <p>$46.50</p>
        </div>
        <div class="confirm-order">
          <p>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="18"
              height="20"
              fill="none"
              viewBox="0 0 21 15"
            >
              <path
                fill="#1EA575"
                d="M8 18.75H6.125V17.5H8V9.729L5.803 8.41l.644-1.072 2.196 1.318a1.256 1.256 0 0 1 .607 1.072V17.5A1.25 1.25 0 0 1 8 18.75Z"
              />
              <path
                fill="#1EA575"
                d="M14.25 18.75h-1.875a1.25 1.25 0 0 1-1.25-1.25v-6.875h3.75a2.498 2.498 0 0 0 2.488-2.747 2.594 2.594 0 0 0-2.622-2.253h-.99l-.11-.487C13.283 3.56 11.769 2.5 9.875 2.5a3.762 3.762 0 0 0-3.4 2.179l-.194.417-.54-.072A1.876 1.876 0 0 0 5.5 5a2.5 2.5 0 1 0 0 5v1.25a3.75 3.75 0 0 1 0-7.5h.05a5.019 5.019 0 0 1 4.325-2.5c2.3 0 4.182 1.236 4.845 3.125h.02a3.852 3.852 0 0 1 3.868 3.384 3.75 3.75 0 0 1-3.733 4.116h-2.5V17.5h1.875v1.25Z"
              />
            </svg>
            This is a <strong>carbon-neutral</strong> delivery
          </p>
        </div>
        <button
          style="
            margin-top: 20px;
            width: 240px;
            border-radius: 30px;
            background-color: hsla(0, 79%, 35%, 0.761);
            font-size: 12px;
            height: 45px;
          "
        >
          Confirm Order
        </button>
      </footer>
    </aside>
  </div>
</template>

<script setup>
import data from "../../../data.json";
</script>

<style lang="scss" scoped>
@import url(../styles/desserts.scss);
@import url(../styles/cart.scss);
</style>

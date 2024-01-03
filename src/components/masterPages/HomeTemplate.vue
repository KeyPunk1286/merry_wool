<template>
  <div class="header">
    <nav class="header__nav">
      <RouterLink to="/">Home</RouterLink>
      <!-- <RouterLink to="/catalog">catalog</RouterLink>
      <RouterLink to="/video">video</RouterLink>
      <RouterLink to="/contact">contact</RouterLink> -->
    </nav>
    <div class="header__actions">
      <div class="actions__input">
        <input type="text" placeholder="search" />
        <UiButtonDefault>
          <UiIconSearch />
        </UiButtonDefault>
      </div>
      <div class="actions__cart">
        <button>
          <UiIconCartEmpty />
        </button>
      </div>
    </div>
  </div>
  <slot></slot>
  <div class="footer">
    <div class="footer__links">
      <a href="#"><img src="@/assets/icon/facebook_logo.png" alt="facebook" /></a>
      <a href="#"><img src="" alt="insta" /></a>
      <a href="#"><img src="" alt="telegram" /></a>
    </div>
  </div>
</template>

<script setup>
import { RouterLink } from 'vue-router'
import UiIconSearch from './ui/UiIconSearch.vue'
import UiIconCartEmpty from './ui/UiIconCartEmpty.vue'
import UiButtonDefault from './ui/UiButtonDefault.vue'
</script>

<style lang="scss" scoped></style>

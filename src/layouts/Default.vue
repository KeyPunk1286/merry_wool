<template>
  <div class="container">
    <header-transparent />
    <slot></slot>
    <the-footer />
  </div>
</template>

<script setup>
import HeaderTransparent from '../components/blocks/HeaderTransparent.vue'
import TheFooter from '../components/blocks/TheFooter.vue'
</script>

<style lang="scss" scoped></style>

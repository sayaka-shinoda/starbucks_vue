<script setup>
  import{ ref } from 'vue'
  import Header from './header.vue'
  import Info from './info.vue'
  import Footer from './footer.vue'
</script>

<template>
  <div class="total">
    <Header />
    <Info />
    <Footer />
  </div>
</template>

<style>
  .total{
    width: 1080px;
  }
</style>
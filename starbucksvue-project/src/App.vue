<script setup>
  import{ ref } from 'vue'
  import Header from './header.vue'
  import Info from './info.vue'
  import Footer from './footer.vue'
</script>

<template>
  <div class="container">
    <Header />
    <Info />
    <Footer />
  </div>
</template>

<style>
  .container{
    width: 1080px;
  }
</style>
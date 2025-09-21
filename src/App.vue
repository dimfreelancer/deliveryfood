<script setup>
import Banner from './components/Banner.vue';
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';

  console.log('hellllo app');
</script>


<template>
  <div class="page-wrapper">
    <Header />
    
    <main class="main">
      <Banner />

      <section class="products">
        <div class="container">
          <router-view></router-view>
        </div>
      </section>
    </main>

    <Footer />
  </div>
</template>


<style scoped>
</style>

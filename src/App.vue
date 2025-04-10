<script setup>
import Caroulsel from './components/Caroulsel.vue';
import Functions from './components/Functions.vue';
import Header from './components/Header.vue';
import Home from './components/Home.vue';
import Prices from './components/Prices.vue';
import Section1 from './components/Section1.vue';
import Duvidas from './components/Duvidas.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <Header></Header>
  <main class="pt-16">
    <Home></Home>
    <Section1></Section1>
    <Functions></Functions>
    <Caroulsel></Caroulsel>
    <Prices></Prices>
    <Duvidas></Duvidas>
    <Footer></Footer>
  </main>
  
</template>

<style scoped>

</style>

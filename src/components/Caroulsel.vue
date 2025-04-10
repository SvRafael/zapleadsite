<template>
    <div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between h-auto space-x-2 py-12">
    <div class="relative w-full h-full mx-auto overflow-hidden rounded-xl shadow-lg">
      
      <!-- Slides -->
      <div
        class="flex transition-transform duration-700 ease-in-out"
        :style="{ transform: `translateX(-${currentIndex * 100}%)` }"
      >
        <div
          v-for="(slide, index) in slides"
          :key="index"
          class="w-full flex-shrink-0"
        >
          <img :src="slide" class="w-full h-max object-cover" />
        </div>
      </div>
  
      <!-- Botões -->
      <button
        @click="prevSlide"
        class="absolute top-1/2 left-4 transform -translate-y-1/2 bg-white/80 hover:bg-white text-gray-800 px-3 py-1 rounded-full shadow"
      >
        ‹
      </button>
  
      <button
        @click="nextSlide"
        class="absolute top-1/2 right-4 transform -translate-y-1/2 bg-white/80 hover:bg-white text-gray-800 px-3 py-1 rounded-full shadow"
      >
        ›
      </button>
  
      <!-- Indicadores -->
      <div class="absolute bottom-4 w-full flex justify-center gap-2">
        <span
          v-for="(slide, index) in slides"
          :key="index"
          class="w-3 h-3 rounded-full"
          :class="currentIndex === index ? 'bg-white' : 'bg-white/50'"
        />
      </div>
    </div>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const slides = ref([
  "https://zapleadoficial.com.br/wp-content/uploads/2025/02/4-1024x640.png",
  "https://zapleadoficial.com.br/wp-content/uploads/2025/02/Selecione-a-etiqueta-desejada-para-que-os-contatos-dessa-etiqueta-possam-ser-listados-para-o-envio-das-mensagem-1024x640.png",
  "https://zapleadoficial.com.br/wp-content/uploads/2025/02/5-1024x640.png",
  "https://zapleadoficial.com.br/wp-content/uploads/2025/02/2-1024x640.png",
  "https://zapleadoficial.com.br/wp-content/uploads/2025/02/Selecione-a-etiqueta-desejada-para-que-os-contatos-dessa-etiqueta-possam-ser-listados-para-o-envio-das-mensagem-1-1024x640.png",
  "https://zapleadoficial.com.br/wp-content/uploads/2025/02/1-1024x640.png",
  "https://zapleadoficial.com.br/wp-content/uploads/2025/02/Selecione-a-etiqueta-desejada-para-que-os-contatos-dessa-etiqueta-possam-ser-listados-para-o-envio-das-mensagem-2-1024x640.png",
  "https://zapleadoficial.com.br/wp-content/uploads/2025/02/Selecione-a-etiqueta-desejada-para-que-os-contatos-dessa-etiqueta-possam-ser-listados-para-o-envio-das-mensagem-4-1024x640.png",
  "https://zapleadoficial.com.br/wp-content/uploads/2025/02/Selecione-a-etiqueta-desejada-para-que-os-contatos-dessa-etiqueta-possam-ser-listados-para-o-envio-das-mensagem-3-1024x640.png"
])
  
  const currentIndex = ref(0)
  
  function nextSlide() {
    currentIndex.value = (currentIndex.value + 1) % slides.value.length
  }
  
  function prevSlide() {
    currentIndex.value =
      (currentIndex.value - 1 + slides.value.length) % slides.value.length
  }
  </script>
  
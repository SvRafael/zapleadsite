<script setup>
import Header from './components/Header.vue';
import Home from './components/Home.vue';
</script>

<template>
  <Header></Header>
  <main class="pt-16">
    <Home></Home>
    
    <section class="bg-gradient-to-b from-green-900 via-green-700 via-green-600 via-green-600 via-green-400 to-green-200 text-white w-full">
      <div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between md:h-[calc(100vh-64px)] h-auto space-x-2">


      <div class="md:w-1/2 w-full">
        <img
          src="https://zapleadoficial.com.br/wp-content/uploads/2025/02/Design-sem-nome-19.png"
          alt="Recrutamento"
          class="w-full h-auto rounded-xl object-cover"
        />
      </div>

      <!-- Texto à direita com fundo branco -->
      <div class="md:w-1/2 w-full bg-white p-8 rounded-xl shadow-md">
        <h2 class="text-3xl font-bold text-gray-800 mb-4">Leve seu atendimento para o próximo nivel!</h2>
        <p class="text-gray-600 text-lg mb-4">
          Responda múltiplas conversas com facilidade, automatize o envio de mensagens e áudios como se fossem gravados na hora, deixando um atendimento leve e humanizado.
        </p>
        <label>ORGANIZAÇÃO = MAIS VENDAS</label>
      </div>

    </div>
  </section>
  </main>
 
</template>

<style scoped>

</style>

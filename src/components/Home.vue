<template>
  <section class="bg-gradient-to-b from-green-900 via-green-200 via-green-600 via-green-600 via-green-700 to-green-900 text-white w-full">
    <div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between md:h-[calc(100vh-64px)] h-auto">

      <!-- Texto à esquerda -->
      <div class="md:w-1/2 w-full p-6 md:p-12">
        <h1 class="text-4xl font-bold bg-gradient-to-r from-green-400 to-green-200 bg-clip-text text-transparent">
        CRM NO WHATSAPP
        </h1>
        <h1 class="text-4xl font-bold mb-4">Transforme conversas em conversoes!</h1>
        <p class="text-lg mb-6">
            Conquiste seus Leads com o poder do ZapLead e aumente suas vendas sem perder o toque humano. Transforme conversas em conversoes!
        </p>
        <a target="_blank" href="https://chromewebstore.google.com/detail/zaplead-transforme-conver/ohekppieeepibkebnlilabljmnkffmof" class="inline-block bg-green-500 hover:text-green-500 text-white font-semibold px-6 py-3 rounded-lg hover:bg-gray-100 transition">
          Saiba mais
        </a>
      </div>

      <!-- Vídeo do YouTube à direita -->
      <div class="md:w-1/2 w-full p-0 m-0">
        <div class="w-full aspect-video">
            <video
                class="w-full h-auto rounded-lg"
                controls
                autoplay
                muted
            >
    <source src="../../public/AULA-2-Instalando-o-ZapLead.mp4" type="video/mp4"/>
    Seu navegador não suporta vídeos .mov. Por favor, baixe o vídeo.
        </video>
        </div>
      </div>

    </div>
  </section>
</template>
  
  <script setup>
  // sem lógica por enquanto, totalmente estático
  </script>
  
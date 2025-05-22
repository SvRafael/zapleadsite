<template>
    <footer class="bg-green-500 text-gray-300 px-6 py-10">
  <section id="footer" class="max-w-7xl mx-auto flex flex-row justify-between  justify-between8">

    <!-- Coluna 1: Institucional -->
    <div class="space-y-3">

            <img
            src="../assets/logo zaplead png branca 2.png"
            alt="ZapLead Logo"
            class="h-32 w-full m-0 p-0 object-cover"
            />
      <p class="text-white">Plataforma de automação, CRM e comunicação humanizada para WhatsApp.</p>
      <p class="text-sm text-white">CNPJ 00.000.000/0001-00</p>
    </div>

    <!-- Coluna 2: Contato -->
    <div class="space-y-3">
      <h3 class="text-white text-lg font-semibold">Contato</h3>
      <p class="text-white font-semibold">Telefone: <a href="tel:+550000000000" class="text-black hover:underline">+55(14) 998496278</a></p>
      <p class="text-white font-semibold">Email: <a href="mailto:contato@zaplead.com.br" class="hover:underline text-black">contato@zaplead.com.br</a></p>
      <a
        href="https://api.whatsapp.com/send?phone=5514998496278&text=OI%C3%A1%2C%20gostaria%20de%20saber%20mais%20sobre%20a%20ferramenta%20ZapLead!"
        target="_blank"
        class="inline-block mt-2 bg-white text-green-600 px-4 py-2 rounded-md transition font-bold"
      >
        Tirar dúvidas no WhatsApp
      </a>
    </div>

    <!-- Coluna 3: Sobre o site -->


  </section>

  <!-- Linha divisória -->
  <div class="border-t border-gray-700 mt-10 pt-6 text-center text-sm text-black">
    <p>
      © {{ new Date().getFullYear() }} ZapLead. Todos os direitos reservados.
    </p>
    <p>
      Site desenvolvido por <a href="https://rafaeldev.net/" class="text-white hover:underline">Simba Sistemas</a>
    </p>
  </div>
</footer>

</template>
<template>
  <section class="h-screen bg-[#F9FAFB] relative pb-24 md:pb-5 lg:pb-5">
    <div class="flex flex-col items-center justify-center h-full text-center">
      <div class="max-w-lg">
        <img src="/logo.png" alt="Logo" class="w-32 mx-auto mb-10" />

        <h1 class="text-4xl font-bold text-[#1D3557] mb-4 px-6">
          Ne laissez plus jamais un cours vous échapper.
        </h1>
        <p class="text-lg text-gray-700 mb-6 px-4">
          Organisez, programmez, et retrouvez vos cours en quelques clics, où que vous soyez.
        </p>
        <button class="bg-[#56CFE1] text-white py-3 px-6 rounded-lg shadow-lg hover:bg-[#3CB1C4] transition duration-200">
          Découvrir l'application
        </button>
      </div>
    </div>
    <img src="/creno.png" alt="Creno" class="absolute bottom-24 sm:bottom-0 right-0 w-[200px] md:w-[300px] lg:w-[500px] m-5" />

    <Footer />
  </section>
</template>

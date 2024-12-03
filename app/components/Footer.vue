<script setup lang="ts">

const email = ref('Un problème ? Ecris-moi : contact@aucreno.com');

function copyEmailToClipboard() {
  const message = 'Un problème ? Ecris-moi : contact@aucreno.com';
  navigator.clipboard.writeText('contact@aucreno.com').then(() => {
    email.value = 'Email copié !';
    setTimeout(() => {
      email.value = message;
    }, 2000);
  }).catch(err => {
    console.error('Erreur lors de la copie : ', err);
  });
};
</script>

<template>
    <div class="hidden sm:flex sm:fixed bottom-0 items-center gap-4 p-4">
      <p @click="copyEmailToClipboard"
        class="text-[10px] text-gray-400 mb-1 hover:text-white transition-colors duration-300 cursor-pointer hover:bg-[#56CFE1] rounded-md px-2 py-1">
        {{ email }}
      </p>
      <NuxtLink to="/privacy"
        class="hidden sm:block text-[10px] text-gray-400 hover:text-white transition-colors duration-300 mb-1 cursor-pointer hover:bg-[#56CFE1] rounded-md px-2 py-1">
        Politique de confidentialité
      </NuxtLink>
      <NuxtLink to="/legal"
        class="hidden sm:block text-[10px] text-gray-400 hover:text-white transition-colors duration-300 mb-1 cursor-pointer hover:bg-[#56CFE1] rounded-md px-2 py-1">
        Mentions légales
      </NuxtLink>
    </div>
</template>
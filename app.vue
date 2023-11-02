<script setup lang="ts">
useHead({
  script: [
    {
      src: 'https://rum.cronitor.io/script.js',
      async: true
    },
    {
      innerHTML: `
        window.cronitor = window.cronitor || function() { (window.cronitor.q = window.cronitor.q || []).push(arguments); };
        cronitor('config', { clientKey: '554a9c7c1b46f81fddea3842771416b0' });
      `
    },
  ]
})
</script>

<template>
  <div class="main">
    <NuxtLayout>
      <NuxtPage/>
    </NuxtLayout>
  </div>
</template>

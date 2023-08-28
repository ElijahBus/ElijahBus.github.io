<script setup lang="ts">
definePageMeta({
  layout: 'default'
});

onMounted(() => {
  navigateTo('https://discord.gg/JQVHpR7P5X', {
    external: true,
    open: {
      target: '_blank'
    }
  });
});
</script>

<template>
  <div class="w-full my-10 text-center">
    <p>Redirecting to the server...</p>
    <p>If you are not automatically redirected, click on the link below or copy and paste it in your browser </p>
    <p>
      <a href="https://discord.gg/JQVHpR7P5X" target="_blank" class="text-blue-900 underline underline-offset-4">
        https://discord.gg/JQVHpR7P5X
      </a>
    </p>

  </div>
</template>
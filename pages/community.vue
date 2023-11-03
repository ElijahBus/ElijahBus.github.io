<script setup lang="ts">
definePageMeta({
  layout: 'default'
});

onMounted(() => {
  navigateTo('https://www.meetup.com/devseccon-kenya/', {
    external: true,
    open: {
      target: '_blank'
    }
  });
});
</script>

<template>
  <div class="w-full mb-10 mt-40 text-center">
    <p>Redirecting to the server...</p>
    <p>If you are not automatically redirected, click on the link below or copy and paste it in your browser </p>
    <p>
      <a href="https://www.meetup.com/devseccon-kenya/" target="_blank" class="text-blue-900 underline underline-offset-4">
        https://www.meetup.com/devseccon-kenya/
      </a>
    </p>

  </div>
</template>
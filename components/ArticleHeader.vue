<script setup lang="ts">

</script>

<template>
  <div class="w-full flex justify-between items-center px-20">
    <div @click="navigateTo('/')" class="cursor-pointer">
      <!-- logo -->
      <img src="/svg/devbus-logo-black.svg" class="" alt="DevBus.Dev Logo" width="100px" />
    </div>

    <div class="navigation-menu">
      <a class="text-sm mx-4 capitalize underline underline-offset-4" href="#">What coming next</a>
      <a class="text-sm mx-4 capitalize underline underline-offset-4" href="#">Podcasts</a>
      <a class="text-sm mx-4 capitalize underline underline-offset-4" href="/articles/event-sourcing-in-nestjs">Your next article to read</a>
      <a class="text-sm mx-4 capitalize underline underline-offset-4" href="mailto:leads@devbus.dev?subject=Hi DevBus.Dev team 👋">CONTACT</a>
      <!--      <a class="bg-blue-900 p-4 text-white text-sm" href="/community">Join The Community</a>-->
    </div>
  </div>
</template>
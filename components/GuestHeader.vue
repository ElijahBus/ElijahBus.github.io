<script setup lang="ts">

</script>

<template>
<!--  <div class="w-full flex justify-between items-center px-20">-->
<!--    <div @click="navigateTo('/')" class="cursor-pointer">-->
<!--      &lt;!&ndash; logo &ndash;&gt;-->
<!--      <img src="/svg/devbus-logo-black.svg" class="" alt="DevBus.Dev Logo" width="100px"/>-->
<!--    </div>-->

<!--    <div class="navigation-menu">-->
<!--      &lt;!&ndash;      <a class="text-sm mx-4 capitalize underline underline-offset-4" href="#">What coming next</a>&ndash;&gt;-->
<!--      &lt;!&ndash;      <a class="text-sm mx-4 capitalize underline underline-offset-4" href="#">Podcasts</a>&ndash;&gt;-->
<!--      <a class="text-sm mx-4 capitalize underline underline-offset-4" href="/articles/event-sourcing-in-nestjs">Your-->
<!--        next article to read</a>-->
<!--      &lt;!&ndash;      <a class="text-sm mx-4 capitalize underline underline-offset-4" href="mailto:leads@devbus.dev?subject=Hi DevBus.Dev team 👋">CONTACT</a>&ndash;&gt;-->
<!--      <a class="bg-blue-900 p-4 text-white text-sm" href="/community">Join The Community</a>-->
<!--    </div>-->
<!--  </div>-->



  <nav class="bg-white dark:bg-gray-900 fixed w-full z-20 top-0 left-0 border-b border-gray-200 dark:border-gray-600">
    <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
      <a href="#" class="flex items-center">
        <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">DevBus.Dev</span>
      </a>
      <div class="flex md:order-2">
        <a href="/community" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-4 py-2 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Join the community</a>
<!--        <button data-collapse-toggle="navbar-sticky" type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-sticky" aria-expanded="false">-->
<!--          <span class="sr-only">Open main menu</span>-->
<!--          <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">-->
<!--            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>-->
<!--          </svg>-->
<!--        </button>-->
      </div>
      <div class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1" id="navbar-sticky">
        <div class="flex flex-col p-4 md:p-0 mt-4 font-medium border border-gray-100 rounded-lg bg-gray-50 md:flex-row md:space-x-8 md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700">
            <a href="/" class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700" aria-current="page">Home</a>
            <a href="/articles/event-sourcing" class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Articles</a>
            <a href="mailto:elijah@devbus.dev"  class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Contact</a>
        </div>
      </div>
    </div>
  </nav>

</template>
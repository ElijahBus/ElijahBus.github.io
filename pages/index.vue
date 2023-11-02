<script setup lang="ts">
definePageMeta({
  layout: 'default'
});

import {useMediaControls} from '@vueuse/core';

const devBusClip = ref();
const {playing, currentTime, volume} = useMediaControls(devBusClip, {
  src: '/video/dev-bus-clip.mp4',
});

onMounted(() => {
  currentTime.value = 0;
  volume.value = 0;

  setTimeout(() => {
    playing.value = !playing.value;
  }, 1000);
});

</script>

<template>
   <div class="flex-1">
     <div class="flex mt-20">
       <!--    <div class="flex-shrink w-1/2 p-10 rounded">-->
       <!--    </div>-->

       <div class="flex-1 text-center">
         <div class="">
           <div class="mt-20">
             <h2 class="text-6xl px-4 leading-snug">
               Let's talk App Security, Discover the best approach to securely ship to production
             </h2>
           </div>

           <div class="mt-10">
             <a href="/articles/event-sourcing" class="text-blue-900 underline underline-offset-4">Find more topics</a>
           </div>
         </div>

       </div>
     </div>

     <div class="w-full mt-10 flex flex-col items-center">
       <h4 class="text-2xl">Brought to you by</h4>

       <div class="mt-4 flex gap-4 items-center">
         <div class="w-[129px] flex flex-col">
           <div class="rounded-full border-2 border-blue-300 p-1">
             <img src="/img/elijahbus.jpg" alt="ElijahBus Picture" class="rounded-full">
           </div>
           <a href="https://twitter.com/elijahbus" class="text-sm mt-2 text-center font-bold">@elijahbus</a>
         </div>

         <div class="w-[129px] flex flex-col">
           <div class="rounded-full border-2 border-blue-300 p-1">
             <img src="/img/devseccon.png" alt="DevSecCon Logo" class="rounded-full">
           </div>
           <a href="https://twitter.com/devseccon" class="text-sm mt-2 text-center font-bold">@devseccon</a>
         </div>
       </div>

     </div>
   </div>


</template>

<style scoped>

</style>
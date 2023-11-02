<script setup lang="ts">

</script>

<template>
  <div class="flex flex-col main-index">
    <GuestHeader />

    <slot></slot>

    <GuestFooter />
  </div>
</template>

<style lang="scss">
.main-index {
  //background-image: url("/img/bg_option_1.jpeg");
  //background-repeat: no-repeat;
  background-size: cover;
}
</style>
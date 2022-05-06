<template>
  <div class="relative  h-full min-h-screen bgimg">
    <!-- <TheNavBar /> -->
    <div class="pt-10 px-10 flex justify-center align-middle">
      <img :width="300" :height="300" src="./assets/logo.png" />
    </div>
    <div class="p-10">
      <router-view class="max-w-xl" />
    </div>

    <div class="pt-10"></div>
    <!-- <TheFooter /> -->
  </div>
</template>

<script>
import TheNavBar from '@/components/TheNavBar';
import TheFooter from '@/components/gem-farm/TheFooter';
export default {
  components: { TheFooter, TheNavBar },
};
</script>

<style>
* {
  font-family: 'Press Start 2P', monospace;
  color: white;
}
input[type='radio']:checked + span {
  @apply text-black;
}
.bgimg {
  background-color: black;
  background-image: url('~@/assets/hero-bricks2.png');
  background-size: 100%;
  background-repeat: no-repeat;
}
</style>

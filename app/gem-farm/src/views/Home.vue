<template>
  <div class="nes-container with-title mb-10">
    <p class="title">Welcome</p>
    <p>Welcome to the cookie farm 💎 - the #1 NFT Staking on Solana!</p>
    <p class="mt-5">
      This front-end is primarily designed for the Farm Manager (most likely the
      dev behind the NFT project). You probably want to build a nicer front-end
      for your stakers (farmers 👩‍🌾).
    </p>
    <p class="mt-5">
      That said, if you're a staker, in theory nothing is stopping you from
      using this front-end to access ALL the farms you're staking with. Simply
      go to the
      <router-link to="/farmer" class="text-blue-700">farmer</router-link> tab
      and enter the farm address (ask your NFT project for it).
    </p>
    <p class="mt-5">
      You can find the docs
      <a class="text-blue-600" href="https://docs.gemworks.gg/" target="_blank"
        >here</a
      >.
    </p>
    <p class="mt-5">
      Gem Farm is deployed at:
      <span class="bg-yellow-100">{{ GEM_FARM_PROG_ID }}</span>
    </p>
  </div>
  <div class="flex flex-row">
    <div class="nes-container with-title flex-1">
      <p class="title">Stake your Cookies</p>
      <p class="mb-5">
        Choose this if you'd like to stake your Cookies.
      </p>
      <router-link to="farmer">
        <button class="nes-btn is-primary">Stake NFTs</button>
      </router-link>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { GEM_FARM_PROG_ID } from '@gemworks/gem-farm-ts';
export default defineComponent({
  setup() {
    return {
      GEM_FARM_PROG_ID,
    };
  },
});
</script>
<style scoped></style>

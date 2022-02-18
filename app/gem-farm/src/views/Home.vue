<template>
  <div class="nes-container with-title mb-10">
    <p class="title">Welcome</p>
    <p>Welcome to the cookie farm 💎 - the #1 NFT Staking on Solana!</p>

    <p class="mt-5">
      $FRTN Farm is deployed at:
      <span class="bg-yellow-100">HdA8vq6B2TTWhdspta1T9uDc5y32MJbQoo1x7KxPVRrv</span>
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

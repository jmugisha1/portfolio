<script setup>
import reel from '@/components/reel.vue'
import chat from '@/components/chat.vue'
import casestudies from '@/components/casestudies.vue'
import hero from '@/components/hero.vue'
import about from '@/components/about.vue'
import inspire from '@/components/inspire.vue'
import resume from '@/components/resume.vue'
</script>

<template>
  <section class="index">
    <reel />
    <hero />
    <about />
    <resume />
    <inspire />
    <casestudies />
    <chat />
  </section>
</template>

<style scoped>
@font-face {
  font-family: 'plaza';
  src: url('../assets/TuxPlaza-Regular.be4f772.woff2') format('woff2');
  font-weight: normal;
  font-style: normal;
}

.index {
  position: relative;
  overflow: hidden;
  /* background-color: red; */
}
</style>

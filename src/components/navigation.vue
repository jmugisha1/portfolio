<script setup></script>

<template>
  <nav class="fixed_nav">
    <p class="hide small-p">mugisha k joel</p>
    <p class="hide small-p">a user experience designer based in kigali</p>
    <div class="fixed_nav_links">
      <button class="button-1">about</button>
      <button class="button-1">case studies</button>
      <button class="button-1">contact</button>
    </div>
  </nav>
</template>

<style scoped>
@font-face {
  font-family: nba;
  src: url(../assets/Fonts/NBAkademieMonoRegular.29a7190.woff2);
}

@media (max-width: 1255px) {
  .fixed_nav {
    .hide {
      display: none;
    }
  }
  .fixed_nav_links {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 12px;
  }
}

@media (min-width: 1256px) {
  .fixed_nav {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    width: 75vw;

    .fixed_nav_links {
      display: flex;
      flex-direction: row;
      height: fit-content;
      gap: 8px;
    }
  }
}
</style>

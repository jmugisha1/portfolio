<script setup></script>

<template>
  <section class="about">
    <div class="about-wrapper">
      <h1 class="h1-big">As</h1>
      <img src="../assets/gif/Group.svg" alt="" class="h1-big-img" />
      <h1 class="h1-big">creative</h1>
      <img src="../assets/gif/st_index_5.gif" alt="" class="h1-big-img" />
      <h1 class="h1-big">developer</h1>
      <h1 class="h1-big">my</h1>
      <h1 class="h1-big">goal</h1>
      <h1 class="h1-big">is</h1>
      <img src="../assets/gif/about-1.gif" alt="" class="h1-big-img" />
      <h1 class="h1-big">to</h1>
      <h1 class="h1-big">designe</h1>
      <h1 class="h1-big">for</h1>
      <h1 class="h1-big">brands</h1>
      <img src="../assets/gif/st_index_4.gif" alt="" class="h1-big-img" />
      <h1 class="h1-big">wanting</h1>
      <h1 class="h1-big">to</h1>
      <h1 class="h1-big">stand</h1>
      <img src="../assets/gif/Vector.svg" alt="" class="svg" />
      <h1 class="h1-big">out</h1>
    </div>
  </section>
</template>

<style scoped>
@font-face {
  font-family: nba;
  src: url(../assets/Fonts/NBAkademieMonoRegular.29a7190.woff2);
}

@font-face {
  font-family: flexa;
  src: url(../assets/Fonts/GT-Flexa-Regular-Trial.woff2);
}

@font-face {
  font-family: basis;
  src: url(../assets/Fonts/BasisGrotesquePro-Regular.woff2);
}
.about {
  min-height: 100vh;
  display: flex;
  align-items: center;
  padding: var(--padding);
  overflow: hidden;
  /*  */

  .about-wrapper {
    width: 100%;
    display: flex;
    align-items: baseline;
    flex-wrap: wrap;

    .svg {
      width: 30vw;
    }
  }
}
</style>

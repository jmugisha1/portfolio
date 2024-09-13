<script setup></script>

<template>
  <div class="fixed_reel">
    <a href="#" class="top">back on top</a>
    <img src="../assets/gif/hero-back.gif" alt="" />
    <div class="fixed_reel_p">
      <p>
        hey am mugisha joel a user experience and motion designer based in
        kigali rwanda
      </p>
    </div>
  </div>
</template>

<style scoped>
@font-face {
  font-family: nba;
  src: url(../assets/Fonts/NBAkademieMonoRegular.29a7190.woff2);
}
* {
  box-sizing: border-box;
}

.top {
  padding: 4px 8px;
  background-color: black;
  text-transform: uppercase;
  position: absolute;
  top: 0;
  left: 0;
  margin: 8px;
  font-size: 12px;
  border-radius: 16px;
  color: #fefefe;
  cursor: pointer;
  font-family: nba;
  z-index: 10000000;
}

@media (max-width: 1023px) {
  .fixed_reel {
    width: calc(100vw - 24px);
    display: flex;
    flex-direction: column;
    border-radius: 8px;
    overflow: hidden;
    position: fixed;
    bottom: 0;
    left: 0;
    z-index: 10000;
    margin: 12px;

    img {
      height: 50vh;
      width: 100%;
      object-fit: cover;
    }

    .fixed_reel_p {
      position: relative;
      background-color: #fefefe;
      padding: 12px;

      p {
        text-transform: uppercase;
        font-size: 14px;
        font-family: nba;
        line-height: 1.3;
      }
    }
  }
}

@media (min-width: 1024px) {
  .fixed_reel {
    width: 356px;
    display: flex;
    flex-direction: column;
    border-radius: 8px;
    overflow: hidden;
    position: fixed;
    right: 0;
    bottom: 0;
    margin: 72px 24px;
    z-index: 10000;
    font-family: nba;
    line-height: 1.3;

    img {
      height: 261px;
      width: 100%;
      object-fit: fill;
    }

    .fixed_reel_p {
      background-color: #fefefe;
      padding: 12px;

      p {
        text-transform: uppercase;
        font-size: 14px;
        color: #121212;
      }
    }
  }
}

@media (max-width: 768px) {
  .fixed_reel {
    width: calc(100vw - 24px);
    display: flex;
    flex-direction: column;
    border-radius: 8px;
    overflow: hidden;
    position: fixed;
    bottom: 0;
    left: 0;
    z-index: 10000;
    margin: 12px;

    video {
      height: 35vh;
      width: 100%;
      object-fit: cover;
    }
  }
}
</style>

<script setup></script>

<template>
  <section class="services">
    <div class="se-title">
      <h1 class="h1-big-xl">super</h1>
      <h1 class="h1-big-xl">powers</h1>
      <p>always casting changes</p>
    </div>
    <div class="se-services">
      <div class="se-wrapper">
        <h3>design + research</h3>
        <p class="par-small">
          from web design to user research, i work with startups and on individual projects to
          design and make educated predictions for their brand identity across all touchpoints.
          working to elevate your business, in this area services include mobile + web design and
          user research
        </p>
        <p class="under">prices starting from 175,000frw</p>
        <p class="under">average timings between 3-4 weeks</p>
      </div>
      <div class="se-wrapper">
        <h3>digital development</h3>
        <p class="par-small">
          when it comes to development i build my websites from the ground up using code to make
          sure that the website is custom and completely bespoke, this includes also e-commerce
          websites or promotional online stores my main tech stack for the job is the good old html,
          css, and vue js as the main framework
        </p>
        <p class="under">prices starting from 250,000frw</p>
        <p class="under">average timings between 4-6 weeks</p>
      </div>
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
  font-family: stone;
  src: url(../assets//Fonts/Blackstone.woff);
}

.services {
  height: 200vh;
  padding: var(--padding);
  .se-title {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border-bottom: 0.2px solid rgb(255, 255, 255, 0.2);

    p {
      font-family: stone;
      color: white;
      font-size: clamp(2.125rem, 1.8438rem + 1.4063vw, 3.25rem);
      text-transform: lowercase;
    }
  }

  .se-services {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;

    h3 {
      font-family: flexa;
      font-size: 26px;
      line-height: 32px;
      letter-spacing: -2.43px;
      text-transform: uppercase;
    }

    .under {
      font-size: 12.5px;
      text-transform: uppercase;
      font-family: nba;
      padding-top: 4px;
      border-top: 0.5px solid rgb(255, 255, 255, 0.5);
    }
  }
}
.services {
  background: linear-gradient(rgb(0, 0, 0, 0.75), rgb(0, 0, 0, 0.75)),
    url('../assets/photos/inspire-back.webp');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  padding: 16px;
  color: white;
}

@media (max-width: 1023px) {
  .se-title {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  /*  */
  .se-services {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 72px;

    .se-wrapper {
      display: flex;
      flex-direction: column;
      width: 100%;
      gap: 12px;
    }
  }
}

@media (min-width: 1024px) {
  .se-services {
    display: flex;
    flex-direction: row;
    justify-content: center;
    gap: 72px;

    .se-wrapper {
      display: flex;
      flex-direction: column;
      gap: 12px;
      width: 27.5vw;
      height: 25vw;

      h3 {
        font-family: flexa;
        font-size: 26px;
        line-height: 32px;
        letter-spacing: -2.43px;
      }

      p {
        font-family: nba;
        font-size: 12px;
        line-height: 1.5;
      }
    }
  }
}
</style>

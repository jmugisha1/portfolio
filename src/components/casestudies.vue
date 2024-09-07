<script setup></script>

<template>
  <section class="casestudies">
    <!--  -->
    <div class="casestudies-title">
      <h1 class="h1-big-xl">case studies</h1>
      <div class="case-sub-title">
        <p class="par-small">below is a list of the <br />projects i have work on</p>
      </div>
    </div>

    <!--  -->
    <div class="casestudies-wrapper">
      <div class="case-rw">
        <RouterLink to="/casestudies/visitrwanda" class="case-open">open casestudy</RouterLink>
        <img src="../assets/photos/exp-rwanda-2.webp" alt="" />

        <p class="case-info">
          experience rwanda, is a case study where i redesigned the visit rwanda vist to give it a
          modern touch and showcase my skills
        </p>
        <p class="case-tags">#web design #copy writing #typography</p>
      </div>
    </div>
  </section>
</template>

<style scoped>
@font-face {
  font-family: nba;
  src: url(../assets/Fonts/NBAkademieMonoRegular.29a7190.woff2);
}
.casestudies {
  /*  */
  .casestudies-title {
    display: flex;
    flex-direction: column;
    height: 100vh;
    justify-content: space-between;
    align-items: center;
    padding: 24px;

    .h1-big-xl,
    .par-small {
      color: black;
      text-align: center;
    }
    .case-sub-title {
      height: 100%;
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
    }
  }

  /*  */
  .casestudies-wrapper {
    padding: var(--padding);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    .case-rw {
      display: flex;
      flex-direction: column;
      gap: 16px;

      a {
        color: white;
        font-size: 14px;
        background-color: black;
        font-family: nba;
        padding: 8px 16px;
        width: fit-content;
        border-radius: 24px;
        cursor: pointer;
      }
      .case-info {
        font-family: flexa;
        font-size: 22px;
        text-transform: capitalize;
      }
      .case-tags {
        font-size: 14px;
        color: rgb(0, 0, 0, 0.75);
        font-family: nba;
        text-transform: uppercase;
      }
    }
  }
}

@media (max-width: 999px) {
  .case-rw {
    img {
      width: 100%;
      height: 915px;
      object-fit: cover;
      border-radius: 24px;
    }
  }
}

@media (min-width: 1000px) {
  .case-rw {
    img {
      width: 744px;
      object-fit: cover;
      border-radius: 24px;
      height: 499px;
    }

    .case-info {
      width: 744px;
    }
  }
}
</style>

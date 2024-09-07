<script setup>
import reel from './reel.vue'
import chat from './chat.vue'
</script>

<template>
  <section class="casestudy_case">
    <reel />
    <!--  -->
    <div class="case-index">
      <div class="case_title">
        <h1 class="h1-big">
          <slot name="casestudy_h1"></slot>
        </h1>
        <RouterLink to="/">[back to home]</RouterLink>
      </div>

      <div class="case-info">
        <p class="case-info-p none">
          <slot name="case-info-p"></slot>
        </p>

        <div class="scroll">
          <p class="small-p">scroll</p>
          <img src="../assets/gif/scroll.gif" alt="" />
        </div>
      </div>
    </div>

    <!--  -->
    <div class="case-imgs-row">
      <slot name="case-imgs-row"></slot>
    </div>

    <!--  -->
    <div class="case-imgs">
      <slot name="case-imgs"></slot>
    </div>
    <chat />
  </section>
</template>

<style scoped>
@font-face {
  font-family: nba;
  src: url(../assets/Fonts/NBAkademieMonoRegular.29a7190.woff2);
}

.casestudy_case {
  overflow: hidden;
  /* background-color: red; */
  /* display: flexbox; */
  /* flex-direction: column; */
  .case-index {
    height: 100vh;
    padding: var(--padding);
    display: flex;
    flex-direction: column;
    justify-content: space-between;

    /*  */
    .case_title {
      display: flex;
      justify-content: space-between;

      a {
        font-family: nba;
        font-size: 14px;
        text-transform: uppercase;
        cursor: pointer;
        white-space: nonwrap;
      }
    }

    /*  */
    .case-info {
      .case-info-p {
        font-family: nba;
        font-size: 14px;
        line-height: 1.4;
        text-transform: uppercase;
      }
      .scroll {
        display: flex;
        gap: 16px;
        p {
          color: black;
          font-size: 14px;
          align-self: flex-end;
        }

        img {
          height: 24px;
          width: 24px;
          filter: brightness(0) saturate(100%);
        }
      }
    }
  }

  /*  */
  .case-imgs {
    display: flex;
    flex-direction: column;
  }
}

@media (max-width: 1023px) {
  .case-info {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    .none {
      display: none;
    }
  }
  .case-imgs-row {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 96px 48px;
    gap: 96px;
    background-color: #010101;
  }
}

@media (min-width: 1024px) {
  .case-info {
    width: 60vw;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    .scroll {
      display: flex;

      gap: 16px;
      p {
        color: black;
        font-size: 14px;
        align-self: flex-end;
      }

      img {
        height: 24px;
        width: 24px;
        filter: brightness(0) saturate(100%);
      }
    }
  }
  .case-imgs-row {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 96px 48px;
    background-color: #010101;
  }
}

@media (max-width: 768px) {
  .case-index {
    .case_title {
      display: flex;
      flex-direction: column-reverse;
      align-items: center;
      gap: 16px;

      .h1-big {
        text-align: center;
      }
    }

    /*  */
  }
}

/* @media screen {
  
} */
</style>

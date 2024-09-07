<script setup>
import navigation from './navigation.vue'
</script>

<template>
  <section class="section-1 flex-1">
    <video muted autoplay loop src="../assets/video/glitch_cropped.mp4" class="video"></video>
    <div class="section-header">
      <navigation />
      <div class="intro">
        <p class="small-p">
          Hi i’m mugisha joel a user experience designer based in kigali rwanda i mainly focus on
          motion, web design and developement.
        </p>
        <br />
        <p class="small-p">
          I do this by combining my keen eye with modern web trends to design appealing visuals
        </p>
      </div>
    </div>

    <!--  -->
    <div class="newstudy">
      <div class="hero_case">
        <RouterLink to="/casestudies/visitrwanda" class="button-1">latest casestudy</RouterLink>
        <div class="opencase"></div>
      </div>
      <div class="scroll">
        <p class="small-p">scroll</p>
        <img src="../assets/gif/scroll.gif" alt="" />
      </div>
    </div>
  </section>
</template>

<style scoped>
.section-1 {
  min-height: 100vh;
  background-color: rgb(0, 0, 0, 0.75);
  overflow: hidden;
  position: relative;

  .section-header {
    display: flex;
    flex-direction: column;
    gap: 36px;
  }

  .newstudy {
    /*  */

    .hero_case {
      .opencase {
        background: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
          url('../assets/photos/ex-rwanda-1.webp');
        height: 43.13vh;
        border-radius: 8px;
        background-size: cover;
        background-position: center;
        padding: 12px;
      }
    }
    /*  */

    .scroll {
      img {
        height: 24px;
        width: 24px;
      }
    }
  }
}

/*  */

@media (max-width: 1024px) {
  .intro {
    P {
      width: 100%;
    }
  }

  .section-1 {
    display: flex;
    flex-direction: column;
    gap: 48px;
    padding: 12px;
    .section-header {
      height: 100vh;
    }

    .newstudy {
      display: flex;
      flex-direction: column;
      gap: 24px;
      width: 100%;

      .hero_case {
        display: flex;
        flex-direction: column;
        gap: 12px;

        .opencase {
          height: 50vh;
          width: 100%;
        }
      }

      .scroll {
        display: none;
      }
    }
  }
}

/*  */
@media (min-width: 1024px) {
  .section-1 {
    padding: 16px;

    .intro {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      gap: 24px;
      width: 76vw;
      P {
        width: 100%;
      }
    }

    /* */

    .newstudy {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: flex-end;
      width: 55vw;

      /* */

      .hero_case {
        display: flex;
        flex-direction: column;
        gap: 12px;

        .opencase {
          width: 356px;
        }
      }

      /* */

      .scroll {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        gap: 8px;
        p {
          align-self: flex-end;
        }
      }
    }
  }
}
</style>

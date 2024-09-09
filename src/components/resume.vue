<script setup></script>

<template>
  <section class="about">
    <!--  -->
    <p class="par-small">about</p>

    <!--  -->
    <div class="ab-about">
      <p class="par-small">
        i joel mugisha am a product designer meaning i do creative work ranging from web & mobile
        design, motion, and user research to front-end development and anything within the ux world.
        <br />
        <br />
        since my early days, i have always felt the urge to create things and bring them to life so
        i am definitely in this career for the love as a designer, i believe good designs are meant
        to inspire and move the target audience meaning i live by this rule when designing, making
        sure my work is not the average boring designs that everyone is doing, aiming at designing
        digital experiences that stand out and leave a lasting impression. in addition to all this
        am a team player ready to collaborate build and deliver all in the name of the client
        <br />
        <br />
        i can't forget to mention i'm a true chelsea fan since day one and love football in general,
        a designer has to have a hobby aye !!
      </p>
      <a
        href="https://drive.google.com/file/d/1EUunU1zaLG-rhEkmOLdwpvpIiGxj1AGz/view?usp=drive_link"
        target="_blank"
        class="button-1"
        >download resume</a
      >
    </div>

    <!--  -->
    <div class="ab-ser">
      <div class="ab-ser-wp">
        <p class="ab-ser-t">design + research</p>
        <p class="ab-ser-p">
          ux/ui design
          <br />
          web design
          <br />
          mobile design
          <br />
          design systems
          <br />
          typography
          <br />
          user personas
        </p>
      </div>
      <div class="ab-ser-wp">
        <p class="ab-ser-t">fron-end development</p>
        <p class="ab-ser-p">
          html + css
          <br />
          javascript + vue js
          <br />
          mantainance
          <br />
          deployement
        </p>
      </div>
    </div>
  </section>
</template>

<style scoped>
@font-face {
  font-family: flexa;
  src: url(../assets/Fonts/GT-Flexa-Regular-Trial.woff2);
}

@font-face {
  font-family: alte;
  src: url(../assets/Fonts/AlteHaasGrotesk-Regular.woff);
}

/*  */
.about {
  padding: var(--padding);
  min-height: 90vh;
  .ab-ser {
    display: flex;
    flex-direction: column;
    gap: 16px;
    font-family: alte;

    .ab-ser-wp {
      display: flex;
      flex-direction: column;
      gap: 12px;

      .ab-ser-t {
        font-size: 13px;
        text-transform: uppercase;
      }

      .ab-ser-p {
        font-size: 13px;
        text-transform: capitalize;
        color: rgb(0, 0, 0, 0.55);
        margin-bottom: 12px;
        line-height: 20px;
      }
    }
  }

  /*  */
  .button-1 {
    color: white;
    font-size: 14px;
    background-color: black;
  }
}

@media (max-width: 560px) {
  .about {
    width: 100%;
    display: flex;
    flex-direction: column;

    .ab-about {
      display: flex;
      flex-direction: column;

      .par-small {
        width: 100%;
      }
    }
  }
}

@media (max-width: 1023px) {
  .about {
    display: flex;
    flex-direction: column;
    gap: 72px;
    margin-right: 25vw;

    .ab-about {
      display: flex;
      flex-direction: column;
      gap: 32px;
    }

    .ab-ser {
      display: flex;
      flex-direction: row;
      width: 100%;
      justify-content: space-between;
    }
  }
}

@media (min-width: 1024px) {
  .about {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin-right: 25vw;

    /**************************************************/
    .ab-about {
      display: flex;
      flex-direction: column;
      gap: 48px;
      font-family: nba;
      font-size: 15px;

      P {
        width: 488px;
        line-height: 1.4;
        text-transform: uppercase;
      }
    }

    /************************************/
    .ab-ser {
      display: flex;
      flex-direction: column;
      gap: 16px;
      font-family: alte;

      .ab-ser-wp {
        display: flex;
        flex-direction: column;
        gap: 12px;

        .ab-ser-t {
          font-size: 13px;
          text-transform: uppercase;
        }

        .ab-ser-p {
          font-size: 13px;
          text-transform: capitalize;
          color: rgb(0, 0, 0, 0.55);
          margin-bottom: 12px;
          line-height: 20px;
        }
      }
    }
  }
}
</style>

<script setup></script>

<template>
  <footer class="chat">
    <div class="chat-footer">
      <p class="par-small par-small-s">
        currently looking for full time employemnt, but also open to freelance projects - copyrights
        reseved mugisha k joel
      </p>
      <div class="chat-links">
        <p class="par-small">email me at</p>
        <p class="par-small under">j.mugisha1@alustudent.com</p>
      </div>
    </div>

    <div class="chat-title">
      <h1 class="h1-big-xl">
        reach out<br />
        and send <br />
        me a chat<br />
      </h1>
    </div>
  </footer>
</template>

<style>
@font-face {
  font-family: flexa;
  src: url(../assets/Fonts/GT-Flexa-Regular-Trial.woff2);
}
.chat {
  background-color: black;
  padding: var(--padding);
  gap: 72px;

  p,
  h1 {
    color: #d371ff;
  }

  .chat-footer {
    .par-small-s {
      width: 50vw;
    }
    .under {
      text-decoration: underline;
    }
  }
}

@media (max-width: 1023px) {
  .chat {
    display: flex;
    flex-direction: column-reverse;

    .chat-footer {
      padding: 24px;
      height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 36px;

      .par-small-s {
        width: 100%;
        text-align: center;
      }

      .chat-links {
        width: 100%;
        display: flex;
        justify-content: space-between;
      }
    }
  }

  /*  */
  .chat-title {
    padding: 24px;
    height: 100vh;
    display: flex;
  }
}

@media (min-width: 1024px) {
  .chat {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    .chat-footer {
      flex-direction: row;
      justify-content: space-between;
    }

    .chat-footer {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;

      .chat-links {
        display: flex;
        flex-grow: 1;
        justify-content: space-between;
      }
    }
  }
}

@media (max-width: 612px) {
  .chat-links {
    display: flex;
    flex-direction: column;
    gap: 24px;
    align-items: center;
  }
}
</style>

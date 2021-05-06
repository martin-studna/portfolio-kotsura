<template>
  <div class="container">
    <main class="main">
      <div
        style="
          flex: 1;
          display: flex;
          justify-content: center;
          align-items: center;
        "
        class="home-video"
      >
        <iframe
          class="home-video"
          width="840"
          height="478"
          src="https://www.youtube.com/embed/VRxG9tCHMqI"
          title="YouTube video player"
          frameborder="0"
          style="border: none"
          allowfullscreen
        ></iframe>
      </div>
      <div style="height: 100%; width: 2px; background-color: white" />
      <div style="flex: 1; color: white; font-family: Montserrat">
        <div style="margin-left: 30px">
          <div style="margin-bottom: 100px; margin-top: 40px">
            <div style="color: #0098fc; font-size: 80px; font-weight: 100">
              JACOB
            </div>
            <div style="font-weight: bold; font-size: 80px">KOTSURA</div>
          </div>
          <div style="font-size: 40px">
            <div
              class="outline-text"
              style="display: flex; flex-direction: column"
            >
              <a href="/design" class="homeLink">BRAND DESIGN</a>
              <a href="/ui" class="homeLink">UX UI DESIGN</a>
              <a href="/animation" class="homeLink">ANIMATION</a>
              <a href="/artwork" class="homeLink">ARTWORK</a>
            </div>
            <div
              style="font-weight: 100; display: flex; flex-direction: column"
            >
              <a href="/about" class="homeLink blue">ABOUT</a>
              <a href="/contact" class="homeLink blue">CONTACT</a>
            </div>
          </div>
          <div
            style="
              color: #2b2b2b;
              text-align: right;
              margin-right: 120px;
              margin-top: 40px;
            "
          >
            by Kotsura and Martin Studna
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'Home',
};
</script>

<style scoped lang="scss">
.container {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: black;
  overflow-x: hidden;
  color: #fff;
}

.main {
  display: flex;
  width: 100%;
  height: 80%;
  justify-content: center;
  background-color: black;
}

.outline-text {
  color: #000;
  font-weight: bold;
  text-shadow: -1px -1px 0 #fff, 1px -1px 0 #fff, -1px 1px 0 #fff,
    1px 1px 0 #fff;
  --webkit-font-smoothing: antialiased;
}

.homeLink {
  height: 60px;
  transition: transform 0.2s linear;
  cursor: pointer;

  &:hover {
    font-style: italic;
    text-shadow: none;
    color: white;
    transform: translate(30px, 0);
  }
}

.blue {
  font-weight: 200;
}

.blue:hover {
  color: $primary;
}

.home-video {
  -webkit-animation: fadein 4s ease-in 10s forwards; /* Safari, Chrome and Opera > 12.1 */
  -moz-animation: fadein 4s ease-in 10s forwards; /* Firefox < 16 */
  -ms-animation: fadein 4s ease-in 10s forwards; /* Internet Explorer */
  -o-animation: fadein 4s ease-in 10s forwards; /* Opera < 12.1 */
  animation: fadein 4s ease-in 10s forwards;
}

@keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Firefox < 16 */
@-moz-keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Safari, Chrome and Opera > 12.1 */
@-webkit-keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Internet Explorer */
@-ms-keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>

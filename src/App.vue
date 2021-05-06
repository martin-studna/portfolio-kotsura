<template>
  <transition name="slide">
    <router-view />
  </transition>
</template>

<style lang="scss">
body {
  margin: 0;
  min-height: 100vh;
  background-color: black;
  display: flex;
  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Oxygen,
    Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, sans-serif;
  overflow-x: hidden;
}

img {
  max-width: 100%;
  display: block;
}

a {
  color: inherit;
  text-decoration: none;
}

* {
  box-sizing: border-box;
}

#app {
  width: 100%;
  flex: 1;
}

.slide-enter-active {
  transition: all 0.5s ease-out;
}
.slide-leave-active {
  transition: all 0.5s ease-out;
}

.slide-enter-from {
  position: absolute;
  left: 100%;
}

.slide-enter-to {
  position: absolute;
  left: 0;
}

.slide-leave-from {
  position: absolute;
  left: -100%;
  opacity: 0;
}

.slide-leave-to {
  position: absolute;
  left: 0;
  opacity: 1;
}
</style>

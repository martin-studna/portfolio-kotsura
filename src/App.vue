<template>
  <transition name="slide">
    <router-view />
  </transition>
</template>

<style lang="scss">
html,
body {
  padding: 0;
  margin: 0;
  width: 100%;
  min-height: 100%;
  background-color: black;
  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Oxygen,
    Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, sans-serif;
  overflow-x: hidden;
  display: flex;
}

a {
  color: inherit;
  text-decoration: none;
}

* {
  box-sizing: border-box;
}

#app {
  height: 100%;
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

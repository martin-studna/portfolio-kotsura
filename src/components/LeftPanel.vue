<template>
  <a href="/">
    <div class="left-panel">
      <div class="left-panel__content">
        <div class="arrow">
          <div class="line-1" />
          <div class="line-2" />
        </div>
        <div class="title">KOTSURA</div>
      </div>
      <div class="left-panel__line"></div>
    </div>
  </a>
</template>

<script>
export default {
  name: 'LeftPanel',
};
</script>

<style lang="scss" scoped>
.left-panel {
  position: relative;
  width: 350px;
  background: black;
  height: 100%;
  display: flex;
  flex-direction: row;

  &:hover .title {
    color: $primary;
  }

  &:hover .line-1,
  &:hover .line-2 {
    background: $primary;
  }

  &__content {
    width: 100%;
    height: 100%;
    position: relative;
  }

  &__line {
    height: 100%;
    width: 10px;
    background: white;
  }
}

.title {
  color: white;
  font-size: 50px;
  font-weight: bold;
  font-family: Montserrat;
  transform: rotate(-90deg);
  position: absolute;
  bottom: 160px;
  right: -111.3px;
}

.arrow {
  position: absolute;
  right: 35px;
  top: 40px;
}

.line-1 {
  position: absolute;
  width: 4px;
  height: 24px;
  background: white;
  transform: rotate(-45deg);
  border-radius: 0.2em;
}

.line-2 {
  position: absolute;
  bottom: -39px;
  width: 4px;
  height: 24px;
  background: white;
  transform: rotate(45deg);
  border-radius: 0.2em;
}
</style>

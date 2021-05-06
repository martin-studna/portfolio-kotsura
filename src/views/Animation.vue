<template>
  <div class="animation">
    <LeftPanel />
    <div class="content">
      <div class="header">
        <div class="header-title">ANIMATION</div>
      </div>
    </div>
    <footer class="footer">
      <a href="/artwork">
        <h5 class="footer-title" style="margin-bottom: 0; margin-top: 0">
          ARTWORK
        </h5>
      </a>
    </footer>
  </div>
</template>

<script>
import LeftPanel from '../components/LeftPanel.vue';

export default {
  name: 'Design',
  components: { LeftPanel },
};
</script>

<style lang="scss" scoped>
.animation {
  width: 100%;
  height: 100%;
  background: black;
  display: flex;
  flex-direction: column;
}

.content {
  width: 100%;
}

.header {
  position: relative;
  height: 200px;
  width: 100%;
  font-weight: bold;
  color: $primary;
  font-family: Montserrat;

  &-title {
    position: absolute;
    right: 10%;
    top: $header-top-align;
    font-size: $header-font-size;
    font-weight: $header-font-weight;
  }
}

.footer {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 100px;
  color: white;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

.footer-title {
  font-family: Montserrat;
  margin-right: 150px;
  font-size: 3.5em;
  font-weight: 800;
  transition: transform 0.2s ease-in;
  cursor: pointer;

  &:hover {
    transform: translate(60px, 0);
    font-style: italic;
    color: $primary;
  }
}
</style>

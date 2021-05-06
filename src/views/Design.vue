<template>
  <div class="design">
    <LeftPanel />
    <div class="content">
      <div class="header">
        <div class="header-title">DESIGN</div>
      </div>
    </div>
    <footer class="footer">
      <h5><a href="/ui">UX UI DESIGN</a></h5>
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
.design {
  width: 100%;
  height: 100%;
  background: white;
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
    right: 0;
    top: $header-top-align;
    font-size: $header-font-size;
    font-weight: $header-font-weight;
    letter-spacing: $header-letter-spacing;
  }
}

.footer {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 100px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

.footer h5 {
  font-family: Montserrat;
  margin-right: 150px;
  font-size: 3.5em;
  font-weight: 800;
  transition: transform 0.2s ease-in;
  cursor: pointer;
}

.footer h5:hover {
  transform: translate(60px, 0);
  font-style: italic;
  color: $primary;
  font-weight: 900 !important;
}
</style>

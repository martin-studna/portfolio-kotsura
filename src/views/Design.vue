<template>
  <div class="design">
    <LeftPanel />
    <div class="content">
      <div class="header">
        <div class="header-title">DESIGN</div>
      </div>
    </div>
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
  flex-direction: row;
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
  }
}
</style>

<template>
  <div class="contact">
    <LeftPanel />
    <div class="content">
      <div class="header">
        <div class="header-title-1">LET'S</div>
        <div class="header-title-2">TALK</div>
      </div>
      <div class="content-body">
        <div class="content-left">
          <img src="../assets/jay_card.png" alt="" class="card" />
        </div>
        <div class="content-right">
          <div>
            <ul class="links">
              <li class="link">
                <a href="">linkedin</a>
              </li>
              <li class="link">
                <a href="">behance</a>
              </li>
              <li class="link">
                <a href="">instagram</a>
              </li>
              <li class="link">
                <a href="">twitter</a>
              </li>
              <li class="link">
                <a href="">facebook</a>
              </li>
              <li class="link">
                <a href="">youtube</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LeftPanel from '../components/LeftPanel.vue';

export default {
  name: 'Contact',
  components: { LeftPanel },
};
</script>

<style lang="scss" scoped>
.contact {
  width: 100%;
  height: 100%;
  background: white;
  display: flex;
  flex-direction: row;
}

.content {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
}

.content-body {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: row;
}

.content-left {
  width: 50%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.content-right {
  background: gray;
  width: 50%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.header {
  position: relative;
  height: 250px;
  width: 100%;
  font-weight: 800;
  color: white;
  font-family: Montserrat;
  background: black;
  box-shadow: 6px 6px 6px #b3b3b3;
  font-size: 180px;

  &-title-1 {
    position: absolute;
    left: 5%;
    top: -20px;
  }
  &-title-2 {
    position: absolute;
    left: 50%;
    bottom: -45px;
  }
}

.card {
  transition: transform 0.2s;
}

.card:hover {
  transform: scale(1.3);
}

.links {
  list-style-type: none;
  color: rgba(0, 0, 0, 0.5);

  font-weight: 900;
  font-size: 60px;
  text-shadow: -1px -1px 0 #fff, 1px -1px 0 #fff, -1px 1px 0 #fff,
    1px 1px 0 #fff;
  --webkit-font-smoothing: antialiased;
}

.link {
}

.link:hover {
  color: #fff;
  text-shadow: none;
  font-weight: 300;
  font-style: italic;
}
</style>

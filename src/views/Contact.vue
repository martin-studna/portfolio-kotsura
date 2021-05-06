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
          <div style="width: 80%">
            <ul class="outline-text links">
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
  margin-left: 222px;
}

.content-body {
  width: 100%;
  height: 100%;
  display: flex;
  margin-top: 15px;
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
  background: rgb(255, 255, 255);
  background: linear-gradient(
    270deg,
    rgba(255, 255, 255, 1) 0%,
    rgba(182, 182, 182, 1) 100%
  );
  width: 50%;
  height: 100%;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}
.outline-text {
  color: #000;
  font-weight: bold;
  text-shadow: -1px -1px 0 #fff, 1px -1px 0 #fff, -1px 1px 0 #fff,
    1px 1px 0 #fff;
  --webkit-font-smoothing: antialiased;
}
.header {
  position: relative;
  height: 32rem;
  width: 100%;
  font-weight: 800;
  color: white;
  font-family: Montserrat;
  background: black;
  /* box-shadow: 6px 6px 6px #b3b3b3; */
  font-size: 300px;

  &-title-1 {
    position: absolute;
    left: 5%;
    top: -20px;
  }
  &-title-2 {
    position: absolute;
    left: 48%;
    bottom: -75px;
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
  margin-right: 3rem;
  font-weight: 900;
  font-size: 100px;
  text-align: center;
}

.link {
  transition: transform 0.2s ease-in;
  /* text-shadow: -1px -1px 0 #fff, 1px -1px 0 #fff, -1px 1px 0 #fff,
    1px 1px 0 #fff;
  --webkit-font-smoothing: antialiased; */
  color: #fff;
}

.link:hover {
  font-style: italic;
  transform: translate(30px, 0);
}
</style>

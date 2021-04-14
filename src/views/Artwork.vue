<template>
  <div class="about">
    <LeftPanel />
    <div class="container">
      <div class="content">
        <div class="header">
          <div class="header-title">ARTWORK</div>
        </div>
        <div class="content-body">
          <div
            style="
              width: 80%;
              display: flex;
              flex-direction: row;
              align-items: center;
              margin-bottom: 120px;
            "
          >
            <img
              style="
                background: transparent;
                border: 1px solid black
                max-width: 500px;
                min-width: 500px;
                height: 400px;
                border-radius: 5px;
                margin-right: 40px;
              "
            />
            <div>
              <h2>ART 1</h2>
              <div class="labels">
                <Label
                  text="original"
                  style="margin-right: 10px"
                  :crossed="true"
                  background="#D6D5D5"
                  color="#A5A3A3"
                />
                <Label text="print" />
              </div>
              <div class="paragraph">
                Talking about artwork etc Talking about artwork etc Talking
                about artwork etc Talking about artwork etc Talking about
                artwork etc Talking about artwork etc
              </div>
              <div class="paragraph">
                Talking about artwork etc Talking about artwork etc Talking
                about artwork etc Talking about artwork etc Talking about
                artwork etc Talking about artwork etc
              </div>
              <div class="paragraph">
                Talking about artwork etcTalking about artwork etc
              </div>
            </div>
          </div>
          <div
            style="
              width: 80%;
              display: flex;
              flex-direction: row;
              align-items: center;
              margin-bottom: 120px;
            "
          >
            <div>
              <h2>ART 1</h2>
              <div class="labels">
                <Label
                  text="original"
                  style="margin-right: 10px"
                  :crossed="true"
                  background="#D6D5D5"
                  color="#A5A3A3"
                />
                <Label text="print" />
              </div>
              <div class="paragraph">
                Talking about artwork etc Talking about artwork etc Talking
                about artwork etc Talking about artwork etc Talking about
                artwork etc Talking about artwork etc
              </div>
              <div class="paragraph">
                Talking about artwork etc Talking about artwork etc Talking
                about artwork etc Talking about artwork etc Talking about
                artwork etc Talking about artwork etc
              </div>
              <div class="paragraph">
                Talking about artwork etcTalking about artwork etc
              </div>
            </div>
            <img
              style="
                background: transparent;
                border: 1px solid black
                max-width: 500px;
                min-width: 500px;
                height: 400px;
                border-radius: 5px;
                margin-right: 40px;
              "
            />
          </div>
          <div
            style="
              width: 80%;
              display: flex;
              flex-direction: row;
              align-items: center;
              margin-bottom: 120px;
            "
          >
            <img
              style="
                background: transparent;
                border: 1px solid black
                max-width: 500px;
                min-width: 500px;
                height: 400px;
                border-radius: 5px;
                margin-right: 40px;
              "
            />
            <div>
              <h2>ART 1</h2>
              <div class="labels">
                <Label
                  text="original"
                  style="margin-right: 10px"
                  :crossed="true"
                  background="#D6D5D5"
                  color="#A5A3A3"
                />
                <Label text="print" />
              </div>
              <div class="paragraph">
                Talking about artwork etc Talking about artwork etc Talking
                about artwork etc Talking about artwork etc Talking about
                artwork etc Talking about artwork etc
              </div>
              <div class="paragraph">
                Talking about artwork etc Talking about artwork etc Talking
                about artwork etc Talking about artwork etc Talking about
                artwork etc Talking about artwork etc
              </div>
              <div class="paragraph">
                Talking about artwork etcTalking about artwork etc
              </div>
            </div>
          </div>
          <div
            style="
              width: 80%;
              display: flex;
              flex-direction: row;
              align-items: center;
              margin-bottom: 120px;
            "
          >
            <div>
              <h2>ART 1</h2>
              <div class="labels">
                <Label
                  text="original"
                  style="margin-right: 10px"
                  :crossed="true"
                  background="#D6D5D5"
                  color="#A5A3A3"
                />
                <Label text="print" />
              </div>
              <div class="paragraph">
                Talking about artwork etc Talking about artwork etc Talking
                about artwork etc Talking about artwork etc Talking about
                artwork etc Talking about artwork etc
              </div>
              <div class="paragraph">
                Talking about artwork etc Talking about artwork etc Talking
                about artwork etc Talking about artwork etc Talking about
                artwork etc Talking about artwork etc
              </div>
              <div class="paragraph">
                Talking about artwork etcTalking about artwork etc
              </div>
            </div>
            <img
              style="
                background: transparent;
                border: 1px solid black
                max-width: 500px;
                min-width: 500px;
                height: 400px;
                border-radius: 5px;
                margin-right: 40px;
              "
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LeftPanel from '../components/LeftPanel.vue';
import Label from '../components/Label.vue';

export default {
  name: 'Artwork',
  components: { LeftPanel, Label },
};
</script>

<style lang="scss" scoped>
.about {
  width: 100%;
  height: 100%;
  background: white;
  display: flex;
  flex-direction: row;
}

.container {
  display: flex;
  justify-content: flex-end;
}

.content {
  right: 0;
  width: 90%;
  height: 100%;
  display: flex;
  justify-content: flex-start;
  flex-direction: column;
}

.content-body {
  width: 100%;
  margin-top: 200px;
}

.header {
  position: relative;
  height: 200px;
  width: 100%;
  font-weight: 800;
  color: $primary;
  font-family: Montserrat;

  &-title {
    position: absolute;
    left: 0;
    top: $header-top-align;
    font-size: $header-font-size;
  }
}

.content-title {
  color: #0098fc;
  font-weight: bold;
  font-size: 60px;
  margin-top: 40px;
  margin-bottom: 40px;
  font-family: Montserrat;
}

.paragraph {
  margin-bottom: 25px;
  font-family: Open Sans;
  font-style: italic;
}

.labels {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  width: 100%;
  margin-bottom: 20px;
}

h2 {
  font-weight: 900;
  font-size: 40px;
}

hr {
  margin-top: 80px;
  margin-bottom: 80px;
  background: #b6b6b6;
  width: 250px;
}
</style>

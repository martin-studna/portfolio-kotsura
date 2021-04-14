<template>
  <div class="about">
    <LeftPanel />
    <div class="container">
      <div class="content">
        <div class="header">
          <div
            style="
              position: absolute;
              color: white;
              font-weight: 100;
              top: 10%;
              left: 10%;
              font-size: 90px;
            "
          >
            JACOB
          </div>
          <div
            style="
              position: absolute;
              color: white;
              font-size: 100px;
              bottom: -12.2%;
              font-weight: bolder;
              left: 30%;
            "
          >
            KOTSURA
          </div>
          <div></div>

          <img
            src="../assets/about-jay-header-photo.png"
            alt=""
            style="height: 100%"
          />
        </div>
        <div class="content-body">
          <div
            style="
              width: 100%;
              display: flex;
              flex-direction: row;
              align-items: center;
            "
          >
            <div
              style="
                background: black;
                max-width: 1250px;
                min-width: 700px;
                height: 500px;
                border-radius: 5px;
                margin-right: 40px;
              "
            ></div>
            <div>
              <div class="paragraph">Hello,</div>
              <div class="paragraph">
                I am Jacob Kotsura a passionate designer and creative from Czech
                Republic.
              </div>
              <div class="paragraph">
                I am focusing mainly on BRANDING, 2D ANIMATION and UX/UI design.
              </div>
            </div>
          </div>
          <div>
            <div class="content-title">EXPERIENCE</div>
            <div
              class="paragraph"
              style="
                display: flex;
                justify-content: flex-end;
                margin-bottom: 70px;
              "
            >
              <img src="../assets/circle_experience.png" alt="" />
            </div>
            <div>
              <div class="paragraph">
                At an early age, I fell in love with creating, and I have been
                practising creative skills since, through elementary art school,
                art and design courses to collage.
              </div>
              <div class="paragraph">
                Being a dedicated learner, I continue taking online courses to
                improve myself and learn useful skills.
              </div>
              <div class="paragraph">
                My freelance career started basically at high school with my
                first design gig. Since then, I helped many businesses create a
                sustainable design for their brand, and now I have over 3 years
                of experience in this field.
              </div>
            </div>
          </div>
          <hr />
          <div>
            <div class="content-title" style="margin-bottom: 0">GOALS</div>
            <div
              style="
                display: flex;
                flex-direction: row;
                justify-content: center;
                align-items: center;
              "
            >
              <img
                src="../assets/profile_about.png"
                alt=""
                style="margin-right: 40px"
              />
              <div style="font-family: Open Sans; font-style: italic">
                My current goal is to work for a studio and at the same time for
                my own clients, to learn how much is possible about the design
                and creative process from both art and business side. And
                hopefully, inspire some people along the way to chase their
                callings and passion.
              </div>
            </div>
          </div>
          <hr style="margin-top: 80px; margin-bottom: 80px" />
          <div>
            <div class="content-title">INSPIRATION</div>
            <div class="paragraph">
              I have many people to consider being my inspiration but to name a
              few of them it would be
            </div>
            <div
              class="paragraph"
              style="
                display: flex;
                justify-content: flex-start;
                align-items: flex-start;
                flex-direction: column;
                padding-left: 20px;
              "
            >
              <div>
                <span
                  style="
                    font-family: Montserrat;
                    font-weight: bold;
                    font-size: 40px;
                    font-style: normal;
                  "
                  >Chris Do</span
                >
                the founder of Blind and the Futur
              </div>
              <div>
                <span
                  style="
                    font-family: Montserrat;
                    font-weight: bold;
                    font-size: 40px;
                    font-style: normal;
                  "
                  >Gary Vee</span
                >
                the marketing genius and funny inspiring guy
              </div>
              <div>
                <span
                  style="
                    font-family: Montserrat;
                    font-weight: bold;
                    font-size: 40px;
                    font-style: normal;
                  "
                  >J.Dvořák
                </span>
                <span style="font-size: 25px; margin-right: 10px">&</span>
                <span
                  style="
                    font-family: Montserrat;
                    font-weight: bold;
                    font-size: 40px;
                    font-style: normal;
                  "
                  >F.Kocura</span
                >
                my two art and life teachers
              </div>
            </div>
          </div>
          <hr />
          <div style="display: flex; flex-direction: row">
            <div style="position: relative">
              <!-- <div style="width: 100%; position: relative">
                <hr style="margin-top: 80px; margin-bottom: 80px" />
              </div> -->
              <div class="content-title">SKILLS</div>
              <div class="paragraph">
                Throughout those years, I have developed the following skillset
                to ensure an in-depth understanding of my field and have the
                best possible results.
              </div>
              <img src="../assets/about_tags.png" alt="" />
            </div>
            <img src="../assets/adobe_icons.png" alt="" />
          </div>
          <hr style="margin-top: 80px; margin-bottom: 80px" />
          <div>
            <div class="content-title" style="margin-botttom: 0 !important">
              PERSONALITY
            </div>
            <div>
              <div>
                <div></div>
                <div></div>
              </div>
              <div>
                <div></div>
                <div></div>
              </div>
            </div>
            <div class="paragraph">
              I love to plan, but I am always ready to learn on the go and take
              on any challenges.
            </div>
            <div class="paragraph">
              The following are the qualities that my clients and employers
              attribute to me.
            </div>
          </div>
          <hr />
          <div>
            <div class="content-title">INTERESTS</div>
            <div class="paragraph" style="margin-bottom: 60px">
              Being a growth-oriented person, I admire exploring and learning
              new ways to create. Besides painting, I enjoy experimenting with
              video and photography as I do love technology. I also possess a
              special affection towards martial arts, and I like to focus on
              complete body movement to ensure better physical health.
            </div>
            <img
              src="../assets/jay_work.png"
              alt=""
              style="margin-bottom: 40px"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LeftPanel from '../components/LeftPanel.vue';

export default {
  name: 'About',
  components: { LeftPanel },
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
  width: 80%;
  margin-top: 75px;
}

.header {
  height: 200px;
  width: 100%;
  box-shadow: 6px 6px 6px #b3b3b3;
  font-weight: bold;
  background: black;
  color: $primary;
  font-family: Montserrat;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  position: relative;

  &-title {
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
  font-family: ppen-Sans;
  font-style: italic;
}

hr {
  margin-top: 80px;
  margin-bottom: 80px;
  background: #b6b6b6;
  width: 250px;
}
</style>

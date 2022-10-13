<template>
  <v-app id="home">
    <navbar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position:relative" class="mt-16">
              <h1 class="wrd">Hello,</h1>
              <h1 class="wrd1">I'M PRATIK SAWANT</h1>
              <span class="wrd2">FRONTED DEVELOPER</span>
              <br />
              <br />
              <v-btn tile dark class="cnt">CONTACT ME</v-btn>
            </div>
          </v-col>
          <v-col cols="2">
            <div class="mtt">
              <v-icon class="white--text">fas fa-angle-double-down</v-icon>
            </div>
          </v-col>
          <v-col cols="5">
            <div class="img1">
              <v-img src="../assets/tom.jpg" contain max-height="400"></v-img>
            </div>
          </v-col>
          <v-col cols="16" class="mt-16" id="about">
            <div>
              <v-row>
                <v-col cols="12" sm="6">
                  <div class="egg">
                    <v-img src="../assets/i2.png"></v-img>
                  </div>
                  <v-col cols="12" sm="6">
                    <h5 class="mt-16">About Me</h5>
                    <div style="width:120px">
                      <v-slider v-model="slider2" color="yellow" label="track-yellow"></v-slider>
                    </div>
                    <h4 class="mt-n4">I Am A Creative Fronted Devloper</h4>
                    <h4 class>And Devloper</h4>
                    <p
                      class="textt"
                    >Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur dicta reiciendis et vel itaque? Praesentium pariatur repellendus perferendis reprehenderit neque eos, rerum vero eveniet, velit harum quasi, quod aperiam. Qui.</p>
                    <br />
                    <p
                      class="textt"
                    >Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque placeat vitae ea consequatur ipsam aperiam provident sapiente commodi vel. Maxime cupiditate dolorum deleniti alias unde aliquam illum temporibus, omnis fugiat.</p>
                    <v-btn tile dark class="dwld">Download Resume</v-btn>
                  </v-col>
                </v-col>
              </v-row>
            </div>
          </v-col>
        </v-row>
      </div>
    </v-container>
  </v-app>
</template>

<style scoped>
.v-container {
  padding: 16px 0px 16px 0px;
}
.head {
  position: inherit;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  width: 100%;
  color: #fff;
}
.head:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: #111111;
  transform: skew(0deg, 6deg);
}
.head:after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg);
}
.cnt {
  color: yellow;
  border-style: inset;
}
.wrd {
  color: grey;
}
.wrd2 {
  color: grey;
}
.mtt {
  position: absolute;
  z-index: 9999;
  bottom: 0;
  margin-right: auto;
  margin-left: auto;
  left: 0;
  right: 0;
  text-align: center;
  margin-top: 16;
  color: #fff;
}
.img1 {
  z-index: 9999;
  position: relative;
  margin-top: 16;
}
.textt {
  color: grey;
}
.dwld {
  color: yellow;
  margin-top: 4;
  border-style: inset;
}
</style>
<script>
import { definecomponent } from "vue";
import Navbar from "@/components/Navbar.vue";

export default {
  name: "Home",

  components: {
    Navbar
  }
};
</script>

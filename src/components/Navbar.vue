<template>
  <v-app-bar app color="black" dark flat class="px-12">
    <v-btn>
      <v-icon color="yellow" left class="mr-2">fas fa-signature</v-icon>PRATIK
    </v-btn>
    <v-spacer></v-spacer>
    <v-btn text @click="scroll('Home')" class="text-yellow">HOME</v-btn>
    <v-btn text @click="scroll('About')">ABOUT</v-btn>
    <v-btn text @click="scroll ('Portfolio')">PORTFOLIO</v-btn>
    <v-btn text @click="scroll ('Services')">SERVICES</v-btn>
    <v-btn text @click="scroll('Page')">PAGE</v-btn>
    <v-btn text @click="scroll('Blog')">BLOG</v-btn>
    <v-btn text @click="scroll('Contact')">CONTACT</v-btn>
  </v-app-bar>
</template>

<style scoped>
</style>
<script>
export default {
  methods: {
    scroll(refName) {
      const element = document.getelementid(refName);
      element.scrollIntoView({ behavior: "smooth" });
    }
  }
};
</script>
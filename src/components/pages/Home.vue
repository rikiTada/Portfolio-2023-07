<script setup>
import AppHeader from "..//globals/AppHeader.vue";
import AppHero from "..//globals/AppHero.vue";
import AppFooter from "..//globals/AppFooter.vue";

import AppProfile from "..//organisms/AppProfile.vue";
import AppContact from "..//organisms/AppContact.vue";

import ScrollDisplay from "..//Atoms/ScrollDisplay.vue";

//=========================================
// GSAP🌟
//=========================================
import gsap from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";
gsap.registerPlugin(ScrollTrigger);
addEventListener("load", () => {
  //=========================================
  // heroFV🌟
  //=========================================
  gsap.set(".gsap", {
    opacity: 1,
  });
  gsap.from(".gsap", {
    duration: 2.5,
    opacity: 0,
    scale: 2,
  });
  gsap.set(".profile", {
    overflow: "hidden",
  });
  //=========================================
  // profile🌟
  //=========================================
  gsap.from(".profile", {
    opacity: 0,
    duration: 1.5,
    scrollTrigger: {
      trigger: "#profile",
      start: "start start",
      markers: true,
    },
  });
});
</script>

<template class="container">
  <AppHeader />
  <main>
    <section id="hero" class="gsap opacity-0">
      <AppHero />
    </section>
    <section id="profile">
      <AppProfile />
    </section>
    <section id="contact">
      <AppContact />
    </section>
  </main>
  <AppFooter />
  <ScrollDisplay />
</template>

<style scoped></style>

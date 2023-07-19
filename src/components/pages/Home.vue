<script setup>
import AppHeader from "..//globals/AppHeader.vue";
import AppHero from "..//globals/AppHero.vue";
import AppFooter from "..//globals/AppFooter.vue";

import AppProfile from "..//organisms/AppProfile.vue";
import AppContact from "..//organisms/AppContact.vue";

import ScrollDisplay from "..//Atoms/ScrollDisplay.vue";
</script>

<template class="container">
  <AppHeader />
  <main>
    <section id="hero">
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

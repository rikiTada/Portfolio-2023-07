<script setup>
import AppHeader from "./components/globals/AppHeader.vue";
import AppHero from "./components/globals/AppHero.vue";
import AppFooter from "./components/globals/AppFooter.vue";

import AppProfile from "./components/organisms/AppProfile.vue";
import AppContact from "./components/organisms/AppContact.vue";

import ScrollDisplay from "./components/Atoms/ScrollDisplay.vue";
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

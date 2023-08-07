<script setup>
import AppMockup from "../molecules/AppMockup.vue";
import AppSvg from "../Atoms/AppSvg.vue";
import SkillList from "../Atoms/SkillList.vue";
</script>
<template>
  <h2 class="section_ttl">PROFILE</h2>
  <div class="flex md:flex-row flex-col justify-center">
    <AppSvg class="pointer-events-none" />
    <div class="text-white tracking-widest">
      <h3 class="text-2xl font-bold hover:after:content-['🙌']">
        Hi, I'm Riki.
      </h3>
      <hr />
      <SkillList
        title="Languages I speak:"
        skills="HTML/CSS, JavaScript, PHP, Python"
      />
      <SkillList title="Frameworks/Libraries:" skills="React, Vue.js, Astro" />

      <SkillList title="Communication Tools:" skills="Notion, Slack" />
      <SkillList
        title="Other Skills:"
        skills="Tailwindcss, SCSS, StoryBook, Figma, WordPress, microCMS"
      />
    </div>
  </div>
  <AppMockup />
</template>

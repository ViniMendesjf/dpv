<script setup lang="ts"></script>
<template>
  <header-section></header-section>
  <body-section></body-section>
  <footer-section></footer-section>
</template>

<style scoped></style>
<script>
import HeaderSection from '@/sections/HeaderSection.vue'
import FooterSection from '@/sections/FooterSection.vue'
import BodySection from '@/sections/BodySection.vue'
export default {
  components: {
    HeaderSection,
    BodySection,
    FooterSection
  }
}
</script>

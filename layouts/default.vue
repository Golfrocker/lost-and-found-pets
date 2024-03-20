<template>
  <AppHeader />
  <NavbarDefault />

  <div>
    <slot />
  </div>

  <AppFooter />
  <div class="translate-y-10"><FooterDefault /></div>
</template>

<script setup>
import FooterDefault from "~/components/FooterDefault.vue";
</script>

<style scoped></style>

<script setup>
import { initFlowbite } from "flowbite";

onMounted(() => {
  initFlowbite();
});
</script>

<template>
  <div class="translate-y-5"><MainCarousel /></div>
  <div class=""><Threecircle /></div>
  <div class="translate-y-5"><Promot /></div>
  <div class="translate-y-5"><Shopindex /></div>
</template>

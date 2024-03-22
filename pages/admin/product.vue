<template>
  <div>
    <Tableproduct />
  </div>
</template>

<script>
import Tableproduct from "~/components/Tableproduct.vue";
definePageMeta({
  layout: "admin",
});

export default {
  components: { Tableproduct },
};
</script>

<style scoped></style>

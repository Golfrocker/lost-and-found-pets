<template>
  <div>
    <Tablepets />
  </div>
</template>

<script>
import Tablepets from "~/components/Tablepets.vue";

definePageMeta({
  layout: "admin",
});

export default {
  components: { Tablepets },
};
</script>

<style></style>

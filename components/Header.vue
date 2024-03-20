<template>
  <div>
    <section
      class="m-2 rounded-2xl shadow-lg shadow-black bg-cover bg-center bg-[url('https://www.maricopa.gov/ImageRepository/Document?documentID=84591')] bg-gray-400 bg-blend-multiply"
    >
      <div class="px-4 mx-auto max-w-screen-xl lg: py-28">
        <h1
          class="text-4xl font-extrabold tracking-tight leading-none text-white md:text-5xl lg:text-6xl uppercase"
        >
          {{ pageTitle }}
        </h1>
      </div>
    </section>
  </div>

  <div><slot /></div>
</template>

<script>
export default {
  data() {
    return {
      pageTitle: "",
    };
  },
  watch: {
    $route(to, from) {
      this.updatePageTitle(to);
    },
  },
  mounted() {
    this.updatePageTitle(this.$route);
  },
  methods: {
    updatePageTitle(route) {
      this.pageTitle = (route.name || "Page Title").toUpperCase();
    },
  },
};
</script>

<style lang="scss" scoped></style>

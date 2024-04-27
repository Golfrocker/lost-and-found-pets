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
      // ตรวจสอบว่ามีชื่อเป็นภาษาไทยหรือไม่ ถ้าไม่มีใช้ "Page Title" แทน
      const thaiNames = {
        about: "เกี่ยวกับ",
        announce: "ประกาศสัตว์เลี้ยงหาย",
        announce2: "ประกาศหาเจ้าของ",
        announce3: "ประกาศหาบ้าน",
        article: "บทความ",
        shop : "สินค้า",
        // เพิ่มชื่อปุ่มที่เป็นภาษาไทยที่ต้องการให้แสดงผลตรงนี้
      };
      const buttonName = route.name;
      this.pageTitle = (thaiNames[buttonName] || "Page Title").toUpperCase();
    },
  },
};
</script>

<style></style>

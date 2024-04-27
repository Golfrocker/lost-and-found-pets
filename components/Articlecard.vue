<template>
  <div class="bg-orange-100 translate-y-5 py-5">
    <div class="text-5xl translate-x-36">บทความ</div>
    <div class="flex justify-around translate-y-5">
      <div class=" grid grid-cols-4 gap-10 px-36 pt-10">
        <div v-for="(card, index) in cards" :key="index" class="mb-4">
          <div
            class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700"
          >
            <img :src="card.image" alt="card image" class="p-8 rounded-t-lg" />
            <div class="p-5">
              <a href="#">
                <h5
                  class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
                >
                  {{ card.title }}
                </h5>
              </a>
              <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
                {{ card.description }}
              </p>
              <a
                href="#"
                class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
              >
                เพิ่มเติม
                <svg
                  class="rtl:rotate-180 w-3.5 h-3.5 ms-2"
                  aria-hidden="true"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 14 10"
                >
                  <path
                    stroke="currentColor"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M1 5h12m0 0L9 1m4 4L9 9"
                  />
                </svg>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cards: [
        {
          title: "10 อุปกรณ์จำเป็น พาน้องหมาเที่ยวต่างจังหวัด",
          description: "อุปกรณ์สำหรับพาน้องหมาเที่ยวต่างจังหวัด",
          image:
            "https://www.petnme.co.th/wp-content/uploads/2024/02/10-essential-for-out-door-dog.webp",
        },
        {
          title:
            "ให้สัตว์เลี้ยงสุขภาพดี.. กับ 5 ไอเท็มเสริมสร้างวิตามินให้หมาแมว",
          description: "ไอเท็มเสริมสร้างวิตามินให้หมาแมว",
          image:
            "https://www.petnme.co.th/wp-content/uploads/2024/02/vitamin-for-pet4.webp",
        },
        {
          title:
            "ปลดปล่อยเอเนอจี้สุดพลัง กับ 3 คอมมูนิตี้เพ็ทเฟรนด์ลี่สำหรับน้องหมา!",
          description: "พี่หมา พาเที่ยว, สุนัข, ไลฟ์สไตล์",
          image:
            "https://www.petnme.co.th/wp-content/uploads/2024/02/community_head.webp",
        },
        {
          title: "ต้นไม้แมวกินได้ ปลูกง่าย มีประโยชน์",
          description: "ต้นไม้ที่ ‘แมว‘ กินได้ แถมดีต่อสุขภาพ!",
          image:
            "https://www.petnme.co.th/wp-content/uploads/2024/02/%E0%B8%95%E0%B9%89%E0%B8%99%E0%B9%84%E0%B8%A1%E0%B9%89%E0%B9%81%E0%B8%A1%E0%B8%A7%E0%B8%81%E0%B8%B4%E0%B8%99%E0%B9%84%E0%B8%94%E0%B9%89-%E0%B8%9B%E0%B8%A5%E0%B8%B9%E0%B8%81%E0%B8%87%E0%B9%88%E0%B8%B2%E0%B8%A2-%E0%B8%A1%E0%B8%B5%E0%B8%9B%E0%B8%A3%E0%B8%B0%E0%B9%82%E0%B8%A2%E0%B8%8A%E0%B8%99%E0%B9%8C_.webp",
        },
      ],
    };
  },
};
</script>

<style scoped></style>

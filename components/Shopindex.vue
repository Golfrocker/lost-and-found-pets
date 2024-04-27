<template>
  <div class="bg-orange-100 translate-y-5 py-5">
    <div class="flex justify-around translate-y-5">
      <div class="text-5xl">สินค้า</div>
      <div>
        <div class="inline-flex rounded-md shadow-sm" role="group">
          <!-- ปุ่มต่าง ๆ สำหรับแสดงสินค้า -->
          <button
            type="button"
            class="px-4 py-2 text-sm font-medium text-gray-900 bg-transparent border border-gray-900 rounded-s-lg hover:bg-gray-900 hover:text-white focus:z-10 focus:ring-2 focus:ring-gray-500 focus:bg-gray-900 focus:text-white dark:border-white dark:text-white dark:hover:text-white dark:hover:bg-gray-700 dark:focus:bg-gray-700"
          >
            สุนัข
          </button>
          <button
            type="button"
            class="px-4 py-2 text-sm font-medium text-gray-900 bg-transparent border-t border-b border-gray-900 hover:bg-gray-900 hover:text-white focus:z-10 focus:ring-2 focus:ring-gray-500 focus:bg-gray-900 focus:text-white dark:border-white dark:text-white dark:hover:text-white dark:hover:bg-gray-700 dark:focus:bg-gray-700"
          >
            แมว
          </button>
          <button
            type="button"
            class="px-4 py-2 text-sm font-medium text-gray-900 bg-transparent border border-gray-900 rounded-e-lg hover:bg-gray-900 hover:text-white focus:z-10 focus:ring-2 focus:ring-gray-500 focus:bg-gray-900 focus:text-white dark:border-white dark:text-white dark:hover:text-white dark:hover:bg-gray-700 dark:focus:bg-gray-700"
          >
            ทั้งหมด
          </button>
        </div>
      </div>
      <nuxt-link to="/shop">
        <div>
          <button class="border-2 border-black px-10 py-4">ดูสินค้า</button>
        </div>
      </nuxt-link>
    </div>
    <div class="grid grid-cols-4 gap-10 px-36 pt-10">
      <div v-for="product in products" :key="product.id" class="flex-grow">
        <div
          class="w-full max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700"
        >
          <img
            :src="product.image"
            alt="product image"
            class="p-8 rounded-t-lg"
          />
          <div class="px-5 pb-5">
            <h6 class="text-gray-500">{{ product.category }}</h6>
            <h5
              class="text-xl font-semibold tracking-tight text-gray-900 dark:text-white"
            >
              {{ product.name }}
            </h5>
            <div class="flex items-center justify-between">
              <span class="text-3xl font-bold text-gray-900 dark:text-white">
                {{ product.price }}
              </span>
              <a
                href="#"
                class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
                >ดูสินค้า</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    const products = [
      {
        id: 1,
        name: "อาหารหมา Zugus",
        category: "สำหรับสุนัข",
        price: "฿599",
        image:
          "https://down-th.img.susercontent.com/file/b7bd0bfeaa4abd95ff013ec7ce164ff9",
      },
      {
        id: 2,
        name: "สายคาด",
        category: "สำหรับแมว",
        price: "฿199",
        image:
          "https://down-th.img.susercontent.com/file/cn-11134301-7r98o-loqkxh4sizrl3e",
      },
      {
        id: 3,
        name: "ของเล่น",
        category: "สำหรับสุนัข",
        price: "฿349",
        image:
          "https://down-th.img.susercontent.com/file/5da16352084d70eb860703d7d8f01de7",
      },
      {
        id: 4,
        name: "กรง",
        category: "สำหรับแมว",
        price: "฿499",
        image:
          "https://down-th.img.susercontent.com/file/th-11134207-7r98z-lsjl2fv3ktim16",
      },
      {
        id: 5,
        name: "อาหารแมว",
        category: "สำหรับแมว",
        price: "฿449",
        image:
          "https://down-th.img.susercontent.com/file/th-11134207-7r98q-lop6y9dbatkt3e",
      },
      {
        id: 6,
        name: "สายจูง",
        category: "สำหรับสุนัข",
        price: "฿99",
        image:
          "https://down-th.img.susercontent.com/file/th-11134207-23030-u0jv5yg8i5nve0",
      },
      {
        id: 7,
        name: "บ้านแมว",
        category: "สำหรับแมว",
        price: "฿1499",
        image:
          "https://down-th.img.susercontent.com/file/th-11134207-7qukw-lk3kf7s8jg9y60",
      },
      {
        id: 8,
        name: "ลูกเต๋า",
        category: "สำหรับสุนัข",
        price: "฿99",
        image:
          "https://down-th.img.susercontent.com/file/th-11134207-7r991-loowyt6tnccd70",
      },
      {
        id: 9,
        name: "ลูกบอลเล่นแมว",
        category: "สำหรับแมว",
        price: "฿79",
        image:
          "https://down-th.img.susercontent.com/file/fa6c3be33dc758deea808d2593817fff",
      },
      {
        id: 10,
        name: "อาหารสัตว์",
        category: "สำหรับสุนัข",
        price: "฿159",
        image:
          "https://down-th.img.susercontent.com/file/a531ae44cc4b8486cc1b97dd771c3e23",
      },
      {
        id: 11,
        name: "อาหารสัตว์",
        category: "สำหรับแมว",
        price: "฿349",
        image: "https://down-th.img.susercontent.com/file/sg-11134201-22100-m5iblwsqohivcc",
      },
      {
        id: 12,
        name: "ของเล่นแมว",
        category: "ของเล่น",
        price: "฿59",
        image: "https://down-th.img.susercontent.com/file/th-11134207-23030-96u55ao1qfov52",
      },
    ];
    return { products };
  },
};
</script>

<style scoped></style>

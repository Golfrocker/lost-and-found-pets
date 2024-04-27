<template>
  <div>
    <div class="relative overflow-x-auto shadow-md sm:rounded-lg">
      <table
        class="w-full text-sm text-left rtl:text-right text-gray-500 dark:text-gray-400"
      >
        <thead
          class="text-xs text-gray-700 uppercase bg-gray-50 dark:bg-gray-700 dark:text-gray-400"
        >
          <tr>
            <th scope="col" class="px-6 py-3">ชื่อสินค้า</th>
            <th scope="col" class="px-6 py-3">รูปภาพ</th>
            <th scope="col" class="px-6 py-3">หมวดหมู่</th>
            <th scope="col" class="px-6 py-3">ราคา</th>
            <th scope="col" class="px-6 py-3">แก้ไข</th>
          </tr>
        </thead>
        <tbody>
          <!-- Mockup data -->
          <tr
            v-for="(product, index) in mockupData"
            :key="index"
            class="bg-white border-b dark:bg-gray-800 dark:border-gray-700"
          >
            <td
              class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white"
            >
              {{ product.name }}
            </td>
            <td class="px-6 py-4">
              <img
                :src="product.image"
                alt="image description"
                class="rounded-full w-20 h-20"
              />
            </td>
            <td class="px-6 py-4">{{ product.category }}</td>
            <td class="px-6 py-4">{{ product.price }}</td>
            <td class="px-6 py-4">
              <a
                href="#"
                class="font-medium text-blue-600 dark:text-blue-500 hover:underline"
                >Edit</a
              >
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      // Mockup data for dogs and cats
      mockupData: [
        {
          name: "Golden Retriever",
          image: "https://via.placeholder.com/150",
          category: "Dog",
          price: "$500",
        },
        {
          name: "Siamese",
          image: "https://via.placeholder.com/150",
          category: "Cat",
          price: "$300",
        },
        {
          name: "Labrador Retriever",
          image: "https://via.placeholder.com/150",
          category: "Dog",
          price: "$450",
        },
        {
          name: "Maine Coon",
          image: "https://via.placeholder.com/150",
          category: "Cat",
          price: "$350",
        },
        {
          name: "German Shepherd",
          image: "https://via.placeholder.com/150",
          category: "Dog",
          price: "$550",
        },
        {
          name: "Persian",
          image: "https://via.placeholder.com/150",
          category: "Cat",
          price: "$400",
        },
        {
          name: "Poodle",
          image: "https://via.placeholder.com/150",
          category: "Dog",
          price: "$600",
        },
        {
          name: "Scottish Fold",
          image: "https://via.placeholder.com/150",
          category: "Cat",
          price: "$320",
        },
        {
          name: "Beagle",
          image: "https://via.placeholder.com/150",
          category: "Dog",
          price: "$480",
        },
        {
          name: "Bengal",
          image: "https://via.placeholder.com/150",
          category: "Cat",
          price: "$380",
        },
      ],
    };
  },
};
</script>

<style scoped></style>

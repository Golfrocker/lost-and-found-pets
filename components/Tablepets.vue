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
            <th scope="col" class="px-6 py-3">ชื่อสัตว์</th>
            <th scope="col" class="px-6 py-3">รูปภาพ</th>
            <th scope="col" class="px-6 py-3">เพศ</th>
            <th scope="col" class="px-6 py-3">อายุ</th>
            <th scope="col" class="px-6 py-3">รางวัล</th>
            <th scope="col" class="px-6 py-3">วันที่หาย</th>
            <th scope="col" class="px-6 py-3"></th>
          </tr>
        </thead>
        <tbody>
          <tr
            v-for="(animal, index) in mockupData"
            :key="index"
            class="bg-white border-b dark:bg-gray-800 dark:border-gray-700"
          >
            <td
              class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white"
            >
              {{ animal.name }}
            </td>
            <td class="px-6 py-4">
              <img
                :src="animal.image"
                alt="image description"
                class="rounded-full w-20 h-20"
              />
            </td>
            <td class="px-6 py-4">{{ animal.gender }}</td>
            <td class="px-6 py-4">{{ animal.age }}</td>
            <td class="px-6 py-4">{{ animal.reward }}</td>
            <td class="px-6 py-4">{{ animal.lostDate }}</td>
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
      mockupData: [
        {
          name: "Dog",
          image: "https://via.placeholder.com/150",
          gender: "Male",
          age: "3 years",
          reward: "$100",
          lostDate: "2024-03-27",
        },
        {
          name: "Dog",
          image: "https://via.placeholder.com/150",
          gender: "Male",
          age: "3 years",
          reward: "$100",
          lostDate: "2024-03-27",
        },
        {
          name: "Cat",
          image: "https://via.placeholder.com/150",
          gender: "Female",
          age: "2 years",
          reward: "$50",
          lostDate: "2024-03-25",
        },
        {
          name: "Rabbit",
          image: "https://via.placeholder.com/150",
          gender: "Male",
          age: "1 year",
          reward: "$20",
          lostDate: "2024-03-24",
        },
        {
          name: "Bird",
          image: "https://via.placeholder.com/150",
          gender: "Unknown",
          age: "6 months",
          reward: "$10",
          lostDate: "2024-03-20",
        },
        {
          name: "Fish",
          image: "https://via.placeholder.com/150",
          gender: "Unknown",
          age: "1 year",
          reward: "$5",
          lostDate: "2024-03-18",
        },
        {
          name: "Hamster",
          image: "https://via.placeholder.com/150",
          gender: "Male",
          age: "1 year",
          reward: "$30",
          lostDate: "2024-03-15",
        },
        {
          name: "Turtle",
          image: "https://via.placeholder.com/150",
          gender: "Female",
          age: "5 years",
          reward: "$80",
          lostDate: "2024-03-10",
        },
        {
          name: "Snake",
          image: "https://via.placeholder.com/150",
          gender: "Male",
          age: "4 years",
          reward: "$70",
          lostDate: "2024-03-05",
        },
        {
          name: "Lizard",
          image: "https://via.placeholder.com/150",
          gender: "Female",
          age: "2 years",
          reward: "$40",
          lostDate: "2024-03-01",
        },
      ],
    };
  },
};
</script>

<style scoped></style>

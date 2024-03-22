<template>
  <div class="px-36 space-y-2">
    <div class="text-4xl">ประกาศสัตว์หาย</div>
    <div>
      <label
        for="small-input"
        class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
        >ชื่อ</label
      >
      <input
        type="text"
        id="small-input"
        class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
      />
    </div>
    <div>
      <label
        for="small-input"
        class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
        >ชื่อ</label
      >
      <input
        type="text"
        id="small-input"
        class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
      />
    </div>
    <label
      for="small-input"
      class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
      >เพศ</label
    >
    <div class="flex">
      <div class="flex items-center me-4">
        <input
          id="inline-checkbox"
          type="checkbox"
          value=""
          class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
        />
        <label
          for="inline-checkbox"
          class="ms-2 text-sm font-medium text-gray-900 dark:text-gray-300"
          >เพศผู้</label
        >
      </div>
      <div class="flex items-center me-4">
        <input
          id="inline-2-checkbox"
          type="checkbox"
          value=""
          class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
        />
        <label
          for="inline-2-checkbox"
          class="ms-2 text-sm font-medium text-gray-900 dark:text-gray-300"
          >เพศเมีย</label
        >
      </div>
    </div>

    <div>
      <label
        for="number-input"
        class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
        >อายุ</label
      >
      <input
        type="number"
        id="number-input"
        aria-describedby="helper-text-explanation"
        class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
        placeholder="อายุ"
        min="0"
        max="99"
        required
      />
    </div>
    <div>
      <label
        for="small-input"
        class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
        >สายพันธุ์</label
      >
      <input
        type="text"
        id="small-input"
        class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
      />
    </div>
    <div>
      <label
        for="small-input"
        class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
        >สี</label
      >
      <input
        type="text"
        id="small-input"
        class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
      />
    </div>
    <div>
      <label
        for="small-input"
        class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
        >รางวัล</label
      >
      <input
        type="text"
        id="small-input"
        class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
      />
    </div>
    <div>
      <label
        for="small-input"
        class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
        >วันที่หาย</label
      >
      <a-date-picker
        v-model:value="value1"
        class="w-full"
        :disabled-date="disabledDate"
      />
    </div>
    <div>
      <label
        for="small-input"
        class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
        >ตำแหน่ง</label
      >
      <input
        type="text"
        id="small-input"
        class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
      />
    </div>
    <label
      for="message"
      class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
      >Your message</label
    >
    <textarea
      id="message"
      rows="4"
      class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
      placeholder="Write your thoughts here..."
    ></textarea>
    <label
      for="small-input"
      class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
      >รูปภาพ</label
    >
    <ImageUpload />
    <button
      type="button"
      class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 me-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 focus:outline-none dark:focus:ring-blue-800"
    >
      Post
    </button>
  </div>
</template>

<script setup>
import { useDayjs } from "#dayjs";
const dayjs = useDayjs();
const disabledDate = (current) => {
  return current && current > dayjs().endOf("day");
};
</script>

<style lang="scss" scoped></style>

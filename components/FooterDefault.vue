<template>
  <footer class="bg-white dark:bg-gray-900">
    <div class="mx-auto w-full max-w-screen-xl p-4 py-6 lg:py-8">
      <div class="md:flex md:justify-between">
        <div class="mb-6 md:mb-0">
          <a href="/" class="flex items-center">
            <img
              src="https://cdn.dribbble.com/users/43762/screenshots/2610432/animals.gif"
              class="rounded-full w-20 h-20 shadow-lg shadow-black"
              alt="Lostandfoundpets Logo"
            />
            <span
              class="self-center text-2xl font-semibold whitespace-nowrap translate-x-5 dark:text-white"
              >LostAndFoundPets</span
            >
          </a>
        </div>
        <div class="grid grid-cols-2 gap-8 sm:gap-6 sm:grid-cols-3">
          <div>
            <h2
              class="mb-6 text-sm font-semibold text-gray-900 uppercase dark:text-white"
            >
              เมนูแนะนำ
            </h2>
            <ul class="text-gray-500 dark:text-gray-400 font-medium">
              <NuxtLink to="/">
                <li class="mb-4">
                  <div class="hover:underline">หน้าเเรก</div>
                </li></NuxtLink
              >
              <NuxtLink to="/announce">
                <li class="mb-4">
                  <div class="hover:underline">ประกาศสัตว์เลี้ยงหาย</div>
                </li></NuxtLink
              >
              <NuxtLink to="/announce2">
                <li class="mb-4">
                  <div class="hover:underline">ประกาศหาบ้าน</div>
                </li></NuxtLink
              >
            </ul>
          </div>
          <div>
            <h2
              class="mb-6 text-sm font-semibold text-gray-900 uppercase dark:text-white"
            >
              <br />
            </h2>
            <ul class="text-gray-500 dark:text-gray-400 font-medium">
              <NuxtLink to="/announce3">
                <li class="mb-4">
                  <div class="hover:underline">ประกาศหาเจ้าของ</div>
                </li></NuxtLink
              >
              <NuxtLink to="/shop">
                <li class="mb-4">
                  <div class="hover:underline">สินค้า</div>
                </li></NuxtLink
              >
            </ul>
          </div>
          <div>
            <h2
              class="mb-6 text-sm font-semibold text-gray-900 uppercase dark:text-white"
            >
              เกี่ยวกับเรา
            </h2>
            <ul class="text-gray-500 dark:text-gray-400 font-medium">
              <NuxtLink to="/article">
                <li class="mb-4">
                  <div class="hover:underline">บทความ</div>
                </li></NuxtLink
              >
              <NuxtLink to="/about">
                <li class="mb-4">
                  <div class="hover:underline">เกี่ยวกับเรา</div>
                </li></NuxtLink
              >
            </ul>
          </div>
        </div>
      </div>
      <hr
        class="my-6 border-gray-200 sm:mx-auto dark:border-gray-700 lg:my-8"
      />
      <div class="sm:flex sm:items-center sm:justify-between">
        <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400"
          >© 2024
          <a href="https://flowbite.com/" class="hover:underline"
            >LostAndFoundPets</a
          >. All Rights Reserved.
        </span>
        <!-- <div class="flex mt-4 sm:justify-center sm:mt-0">
          <NuxtLink to="https://line.me/R/ti/p/@064yhomx?from=page&accountId=064yhomx">
            <img
              src="https://petnme.co.th/wp-content/uploads/2024/02/PET-N-ME-LINE.webp"
              alt=""
              class="h-12"
          /></NuxtLink>
        </div> -->
      </div>
    </div>
    <slot />
  </footer>
</template>

<script setup></script>

<style scoped></style>

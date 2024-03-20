<template>
  <div>
    <div class="flex justify-around">
      <div class="text-3xl">Pet Foodies</div>
      <div>2</div>
      <div>
        <button class="border-2 border-black px-10 py-4">Shop now</button>
      </div>
    </div>
    <div class="grid grid-cols-4 gap-10 px-36 pt-10">
      <div v-for="i in 8" :key="i">
        <div
          class="w-full max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700"
        >
          <a href="#">
            <img
              class="p-8 rounded-t-lg"
              src="data:image/jpeg;base64,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"
              alt="product image"
            />
          </a>
          <div class="px-5 pb-5">
            <a href="#">
              <h5
                class="text-xl font-semibold tracking-tight text-gray-900 dark:text-white"
              >
                Apple Watch Series 7 GPS, Aluminium Case, Starlight Sport
              </h5>
            </a>
            <div class="flex items-center mt-2.5 mb-5">
              <div class="flex items-center space-x-1 rtl:space-x-reverse">
                <svg
                  class="w-4 h-4 text-yellow-300"
                  aria-hidden="true"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="currentColor"
                  viewBox="0 0 22 20"
                >
                  <path
                    d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
                  />
                </svg>
                <svg
                  class="w-4 h-4 text-yellow-300"
                  aria-hidden="true"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="currentColor"
                  viewBox="0 0 22 20"
                >
                  <path
                    d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
                  />
                </svg>
                <svg
                  class="w-4 h-4 text-yellow-300"
                  aria-hidden="true"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="currentColor"
                  viewBox="0 0 22 20"
                >
                  <path
                    d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
                  />
                </svg>
                <svg
                  class="w-4 h-4 text-yellow-300"
                  aria-hidden="true"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="currentColor"
                  viewBox="0 0 22 20"
                >
                  <path
                    d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
                  />
                </svg>
                <svg
                  class="w-4 h-4 text-gray-200 dark:text-gray-600"
                  aria-hidden="true"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="currentColor"
                  viewBox="0 0 22 20"
                >
                  <path
                    d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
                  />
                </svg>
              </div>
              <span
                class="bg-blue-100 text-blue-800 text-xs font-semibold px-2.5 py-0.5 rounded dark:bg-blue-200 dark:text-blue-800 ms-3"
                >5.0</span
              >
            </div>
            <div class="flex items-center justify-between">
              <span class="text-3xl font-bold text-gray-900 dark:text-white"
                >$599</span
              >
              <a
                href="#"
                class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
                >Add to cart</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>

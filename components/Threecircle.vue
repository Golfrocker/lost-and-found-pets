<template>
  <div class="flex justify-around px-36 pt-24">
    <NuxtLink to="/announce">
      <div class="space-y-5 object-cover">
        <img
          class="w-60 h-60 rounded-full shadow-lg shadow-black"
          src="https://png.pngtree.com/png-clipart/20210912/original/pngtree-lost-dog-cartoon-illustration-sns-png-image_6771630.jpg"
          alt=""
        />
        <div class="text-xl text-black text-center font-semibold">
          ประกาศสัตว์เลี้ยงหาย
        </div>
      </div>
    </NuxtLink>

    <NuxtLink to="/announce2">
      <div class="space-y-5">
        <img
          class="w-60 h-60 rounded-full object-cover shadow-lg shadow-black"
          src="https://thumb.ac-illust.com/cd/cd29b875987a8c68288ffffe4dab18a6_t.jpeg"
          alt=""
        />
        <div class="text-xl text-black text-center font-semibold">
          ประกาศหาเจ้าของ
        </div>
      </div>
    </NuxtLink>

    <NuxtLink to="/announce3">
      <div class="space-y-5">
        <img
          class="w-60 h-60 rounded-full object-cover shadow-lg shadow-black"
          src="https://media.istockphoto.com/id/1285935577/th/%E0%B9%80%E0%B8%A7%E0%B8%84%E0%B9%80%E0%B8%95%E0%B8%AD%E0%B8%A3%E0%B9%8C/%E0%B9%84%E0%B8%AD%E0%B8%84%E0%B8%AD%E0%B8%99%E0%B8%A3%E0%B9%89%E0%B8%B2%E0%B8%99%E0%B8%82%E0%B8%B2%E0%B8%A2%E0%B8%AA%E0%B8%B1%E0%B8%95%E0%B8%A7%E0%B9%8C%E0%B9%80%E0%B8%A5%E0%B8%B5%E0%B9%89%E0%B8%A2%E0%B8%87-%E0%B8%9A%E0%B9%89%E0%B8%B2%E0%B8%99%E0%B8%AB%E0%B8%A1%E0%B8%B2-%E0%B8%AD%E0%B8%B8%E0%B8%9B%E0%B8%81%E0%B8%A3%E0%B8%93%E0%B9%8C%E0%B9%80%E0%B8%AA%E0%B8%A3%E0%B8%B4%E0%B8%A1%E0%B8%AA%E0%B9%8D%E0%B8%B2%E0%B8%AB%E0%B8%A3%E0%B8%B1%E0%B8%9A%E0%B8%AA%E0%B8%B1%E0%B8%95%E0%B8%A7%E0%B9%8C%E0%B9%80%E0%B8%A5%E0%B8%B5%E0%B9%89%E0%B8%A2%E0%B8%87-%E0%B8%A0%E0%B8%B2%E0%B8%9E%E0%B8%9B%E0%B8%A3%E0%B8%B0%E0%B8%81%E0%B8%AD%E0%B8%9A%E0%B9%80%E0%B8%A7%E0%B8%81%E0%B9%80%E0%B8%95%E0%B8%AD%E0%B8%A3%E0%B9%8C%E0%B9%83%E0%B8%99%E0%B8%A0%E0%B8%B2%E0%B8%9E%E0%B8%95%E0%B8%B1.jpg?s=612x612&w=0&k=20&c=FS8EmvOnATpV1nJcOyHFnYBOtaM_5QpAWtrjv3f-YBg="
          alt=""
        />
        <div class="text-xl text-black text-center font-semibold">
          ประกาศหาบ้าน
        </div>
      </div>
    </NuxtLink>
  </div>
  <div><slot /></div>
</template>

<script setup></script>

<style scoped></style>

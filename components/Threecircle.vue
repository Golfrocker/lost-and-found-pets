<template>
  <div class="flex justify-around px-36 pt-24">
    <div v-for="i in 3" :key="i">
      <div class="space-y-5">
        <img
          class="w-60 h-60 rounded-full object-cover"
          src="https://www.thesprucepets.com/thmb/UX4NHGthaE9DepYeTzaUh06yxFE=/1500x0/filters:no_upscale():strip_icc()/GettyImages-137068117-6f02b63483df4a2eb95d51bb9b487d0f.jpg"
          alt=""
        />
        <div class="text-xl text-black text-center font-semibold">asdsd</div>
        <div class="text-center text-black/75">asdsad</div>
      </div>
    </div>
  </div>
  <div><slot /></div>
</template>

<script setup></script>

<style scoped></style>

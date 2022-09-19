<template>
  <div class="w-24 pt-2 flex flex-col items-center">
    <div class="font-semibold text-center">DISCORD</div>

    <icon-wrapper class="group transition-all hover:bg-indigo-500">
      <i class="bx bxl-discord-alt text-3xl group-hover:text-white"></i>
    </icon-wrapper>

    <icon-wrapper class="group transition-all hover:bg-blue-500">
      <i class="bx bxs-smile text-3xl group-hover:text-white"></i>
    </icon-wrapper>

    <span class="h-0.5 bg-gray-500 w-1/2 mt-2 rounded-lg" />

    <icon-wrapper class="group transition-all hover:bg-white">
      <i class="bx bxs-joystick text-3xl group-hover:text-black"></i>
    </icon-wrapper>

    <icon-wrapper class="group transition-all hover:bg-green-500">
      <i class="bx bx-plus text-3xl text-green-500 group-hover:text-white"></i>
    </icon-wrapper>

    <icon-wrapper class="group transition-all hover:bg-green-500">
      <i
        class="bx bx-search text-3xl text-green-500 group-hover:text-white"
      ></i>
    </icon-wrapper>
  </div>
</template>

<script>
import IconWrapper from "./IconWrapper.vue";
export default {
  components: { IconWrapper },
};
</script>

<style lang="scss" scoped>
</style>
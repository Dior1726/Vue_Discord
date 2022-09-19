<template>
  <div
    id="app"
    class="
      bg-black-1
      py-2
      px-2
      text-white
      absolute
      top-0
      left-0
      right-0
      bottom-0
      flex
      gap-2
    "
  >
    <left-menu />
    <router-view />
  </div>
</template>

<script>
import LeftMenu from "@/components/LeftMenu.vue";
export default {
  components: {
    LeftMenu,
  },
};
</script>
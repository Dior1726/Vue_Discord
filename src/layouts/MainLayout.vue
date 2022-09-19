<template>
  <div
    class="
      w-full
      flex-grow flex flex-col
      rounded-xl
      bg-black-2
      min-h-0
      overflow-hidden
      mt-5
    "
  >
    <top-header />

    <div class="w-full flex-grow flex min-h-0">
      <left-sidebar />

      <main
        class="flex-grow flex flex-col relative min-h-0 bg-black-3 px-5 py-2"
        style="min-width: 400px"
      >
        <router-view />
      </main>

      <right-sidebar />
    </div>
  </div>
</template>


<script>
import TopHeader from "@/components/Header.vue";
import RightSidebar from "@/components/RightSidebar.vue";
import LeftSidebar from "@/components/LeftSIdebar.vue";

export default {
  components: {
    TopHeader,
    LeftSidebar,
    RightSidebar,
  },
};
</script>

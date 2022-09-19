<template>
  <div class="mt-4">
    <div class="uppercase cursor-pointer select-none py-1" @click="toggleMenu">
      <i
        class="bx bx-chevron-down transform transition-all"
        :class="{ 'rotate-180': isOpen }"
      ></i>
      {{ item.title }}
    </div>

    <div v-show="isOpen">
      <div
        v-for="link in item.child"
        :key="link.id"
        class="
          pl-4
          mb-2
          text-gray-400
          lowercase
          transition-all
          hover:text-white
        "
      >
        <i class="bx bx-hash"></i>
        {{ link.title }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["item"],
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>

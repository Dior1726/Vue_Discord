<template>
  <div
    class="
      w-10
      h-10
      bg-black-3
      flex
      items-center
      justify-center
      mt-2
      rounded-full
      relative
      border border-black
    "
    :class="[isOnline ? 'bg-green-500' : 'bg-gray-500']"
  >
    <i :class="`${iconName} ${size || ''}`"></i>
    <span
      class="absolute bottom-0 right-0 w-4 h-4 rounded-full border border-black"
      :class="[isOnline ? 'bg-green-500' : 'bg-red-500']"
    />
  </div>
</template>

<script>
export default {
  props: ["iconName", "size", "isOnline"],
  data() {
    return {};
  },
};
</script>
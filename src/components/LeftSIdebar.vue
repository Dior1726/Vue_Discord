<template>
  <div
    class="w-60 bg-black-2 pt-4 pr-1 flex-grow flex flex-col relative min-h-0"
    style="min-width: 15rem; max-width: 15rem"
  >
    <div class="px-2 flex-grow flex flex-col overflow-y-auto min-h-0 pb-20">
      <button
        class="
          flex
          w-full
          justify-between
          items-center
          p-2
          bg-black-4
          rounded-lg
          mb-5
        "
      >
        <span class="flex items-center gap-2">
          <i class="bx bx-hash text-gray-400 text-xl"></i>
          welcome
        </span>
        <i class="bx bxs-user-plus text-gray-400 text-xl"></i>
      </button>

      <menu-dropdown v-for="(item, n) in menu" :key="n" :item="item" />
    </div>

    <div
      class="
        absolute
        bottom-0
        left-0
        right-0
        flex
        items-center
        gap-4
        bg-black-5
        w-full
        p-3
      "
    >
      <profile-wrapper
        :isOnline="true"
        :iconName="'bx bxl-discord-alt'"
        :size="'text-2xl'"
      />
      <div class="flex flex-col">
        <span class="text-sm">LO4D.com</span>
        <span class="text-sm">#123s</span>
      </div>
      <div class="flex gap-3 text-gray-400">
        <i class="bx bx-microphone hover:text-gray-300"></i>
        <i class="bx bx-support hover:text-gray-300"></i>
        <i class="bx bxs-cog hover:text-gray-300"></i>
      </div>
    </div>
  </div>
</template>

<script>
import MenuDropdown from "./MenuDropdown.vue";
import ProfileWrapper from "./ProfileWrapper.vue";
export default {
  components: {
    ProfileWrapper,
    MenuDropdown,
  },
  data() {
    return {
      menu: [
        {
          id: 1,
          title: "Info",
          child: [
            {
              id: Math.round(Math.random() * 10000),
              title: "rules",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "Hello",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "feedback",
            },
          ],
        },
        {
          id: 2,
          title: "ACTIvites",
          child: [
            {
              id: Math.round(Math.random() * 10000),
              title: "rules",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "Hello",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "feedback",
            },
          ],
        },
        {
          id: 3,
          title: "loungers",
          child: [
            {
              id: Math.round(Math.random() * 10000),
              title: "rules",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "Hello",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "feedback",
            },
          ],
        },
        {
          id: 12,
          title: "Info",
          child: [
            {
              id: Math.round(Math.random() * 10000),
              title: "rules",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "Hello",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "feedback",
            },
          ],
        },
        {
          id: 23,
          title: "ACTIvites",
          child: [
            {
              id: Math.round(Math.random() * 10000),
              title: "rules",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "Hello",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "feedback",
            },
          ],
        },
        {
          id: 334,
          title: "loungers",
          child: [
            {
              id: Math.round(Math.random() * 10000),
              title: "rules",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "Hello",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "feedback",
            },
          ],
        },
        {
          id: 3324,
          title: "New",
          child: [
            {
              id: Math.round(Math.random() * 10000),
              title: "rules",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "Hello",
            },
            {
              id: Math.round(Math.random() * 10000),
              title: "feedback",
            },
          ],
        },
      ],
    };
  },
  methods: {},
};
</script>
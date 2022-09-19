<template>
  <div
    class="w-60 bg-black-2 pt-4 pr-1 flex-grow flex flex-col relative min-h-0"
    style="min-width: 15rem; max-width: 15rem"
  >
    <div class="px-2 flex-grow flex flex-col overflow-y-auto min-h-0 pb-20">
      <user-list-component
        v-for="(item, n) in allUsers"
        :key="n"
        :item="item"
      />
    </div>
  </div>
</template>

<script>
import MenuDropdown from "./MenuDropdown.vue";
import ProfileWrapper from "./ProfileWrapper.vue";
import UserListComponent from "./UserListComponent.vue";
export default {
  components: {
    ProfileWrapper,
    MenuDropdown,
    UserListComponent,
  },
  data() {
    return {
      allUsers: [
        {
          id: Math.round(Math.random() * 1000000),
          userType: "b.o.t",
          users: [
            {
              id: Math.round(Math.random() * 1000000),
              name: "DAnr Me",
              playArea: "Play",
              isOnline: true,
              isBot: true,
              profileImage: "bx bxl-discord-alt",
            },
            {
              id: Math.round(Math.random() * 1000000),
              name: "Drake",
              playArea: "Play",
              isOnline: true,
              isBot: true,
              profileImage: "bx bxl-discord-alt",
            },
            {
              id: Math.round(Math.random() * 1000000),
              name: "S1mple",
              playArea: "",
              isOnline: true,
              isBot: true,
              profileImage: "bx bxl-discord-alt",
            },
          ],
        },
        {
          id: Math.round(Math.random() * 1000000),
          userType: "The members",
          users: [
            {
              id: Math.round(Math.random() * 1000000),
              name: "DAnr Me",
              playArea: "Play",
              isOnline: true,
              isBot: false,
              profileImage: "bx bxl-discord-alt",
            },
            {
              id: Math.round(Math.random() * 1000000),
              name: "Drake",
              playArea: "Play",
              isOnline: false,
              isBot: false,
              profileImage: "bx bxl-discord-alt",
            },
            {
              id: Math.round(Math.random() * 1000000),
              name: "S1mple",
              playArea: "",
              isOnline: true,
              isBot: false,
              profileImage: "bx bxl-discord-alt",
            },
          ],
        },
        {
          id: Math.round(Math.random() * 1000000),
          userType: "offline",
          users: [
            {
              id: Math.round(Math.random() * 1000000),
              name: "DAnr Me",
              playArea: "Play",
              isOnline: false,
              isBot: false,
              profileImage: "bx bxl-discord-alt",
            },
            {
              id: Math.round(Math.random() * 1000000),
              name: "Drake",
              playArea: "Play",
              isOnline: false,
              isBot: false,
              profileImage: "bx bxl-discord-alt",
            },
            {
              id: Math.round(Math.random() * 1000000),
              name: "S1mple",
              playArea: "",
              isOnline: false,
              isBot: false,
              profileImage: "bx bxl-discord-alt",
            },
          ],
        },
      ],
    };
  },
  methods: {},
};
</script>
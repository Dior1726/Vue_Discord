<template>
  <div class="w-full flex flex-col">
    <div class="uppercase mb-1 mt-2">
      {{ item.userType }} - {{ item.users.length }}
    </div>

    <div class="w-full flex flex-col mb-4">
      <div
        v-for="user in item.users"
        :key="user.id"
        class="w-full flex items-center gap-4"
      >
        <profile-wrapper
          :iconName="user.profileImage"
          :isOnline="user.isOnline"
          :size="'text-2xl'"
        />
        <div class="flex flex-col">
          <span
            class="font-bold"
            :class="[user.isOnline ? 'text-green-700' : ' text-yellow-700']"
          >
            {{ user.name }}
          </span>
          <span class="text-xs text-gray-400"> {{ user.playArea }} </span>
        </div>
        <div class="text-xs p-1 bg-main rounded-md" v-if="user.isBot">BOT</div>
      </div>
    </div>
  </div>
</template>

<script>
import ProfileWrapper from "./ProfileWrapper.vue";
export default {
  props: ["item"],
  components: {
    ProfileWrapper,
  },
};
</script>

<style lang="scss" scoped>
</style>
<template>
  <div class="relative flex-grow flex flex-col min-h-0">
    <div
      class="
        container
        flex-grow flex flex-col
        overflow-y-auto
        minh
        mx-auto
        mt-10
        pb-20
        mb-10
      "
    >
      <h1
        class="
          text-center text-3xl text-main-light
          font-semibold
          uppercase
          mb-10
        "
      >
        Welcome to the server!
      </h1>

      <div class="max-w-sm mx-auto">
        <div class="mb-10 flex items-center gap-10">
          <div><i class="text-5xl text-main-light bx bx-error-circle"></i></div>
          <div class="text-lg text-gray-400">
            <b>Lorem ipsum dolor,</b> sit amet consectetur adipisicing elit.
            Veritatis, id.
          </div>
        </div>

        <div class="mb-10 flex items-center gap-10">
          <div><i class="text-5xl text-main-light bx bxs-user-plus"></i></div>
          <div class="text-lg text-gray-400">
            <b>Lorem ipsum dolor,</b> sit amet consectetur adipisicing elit.
            Veritatis, id.
          </div>
        </div>

        <div class="mb-10 flex items-center gap-10">
          <div><i class="text-5xl text-main-light bx bx-mobile"></i></div>
          <div class="text-lg text-gray-400">
            <b>Lorem ipsum dolor,</b> sit amet consectetur adipisicing elit.
            Veritatis, id.
          </div>
        </div>

        <div class="mb-10 flex items-center gap-10">
          <div><i class="text-5xl text-main-light bx bxl-twitter"></i></div>
          <div class="text-lg text-gray-400">
            <b>Lorem ipsum dolor,</b> sit amet consectetur adipisicing elit.
            Veritatis, id.
          </div>
        </div>
      </div>
    </div>

    <div
      class="
        w-full
        flex
        items-center
        gap-4
        p-4
        bg-black-4
        rounded-lg
        absolute
        left-0
        right-0
        bottom-0
        bg-black-3
      "
    >
      <div>
        <i
          class="bx bxs-plus-circle text-2xl text-gray-400 hover:text-gray-300"
        ></i>
      </div>
      <input
        class="border-none bg-transparent outline-none flex-1"
        placeholder="Message #welcome"
        type="text"
      />
      <div>
        <i class="bx bxs-gift text-2xl text-gray-400 hover:text-gray-300"></i>
      </div>
      <div>
        <i
          class="bx bxs-file-gif text-2xl text-gray-400 hover:text-gray-300"
        ></i>
      </div>
      <div>
        <i class="bx bxs-smile text-2xl text-gray-400 hover:text-gray-300"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>
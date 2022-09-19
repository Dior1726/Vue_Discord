<template>
  <div class="h-14 flex border-b border-black border-opacity-10 shadow-lg">
    <div class="w-60 h-full bg-black-2 p-4">Game Center</div>
    <div
      class="flex-1 h-full bg-black-3 flex items-center justify-between px-4"
    >
      <div class="flex items-center gap-2">
        <i class="bx bx-hash text-2xl text-gray-400"></i>
        <span>welcome</span>
      </div>

      <div class="flex items-center gap-3 text-xl">
        <div><i class="bx bxs-bell text-gray-400 hover:text-gray-300"></i></div>
        <div><i class="bx bx-pin text-gray-400 hover:text-gray-300"></i></div>
        <div>
          <i class="bx bxs-user-detail text-gray-400 hover:text-gray-300"></i>
        </div>
        <div
          class="
            flex
            items-center
            gap-2
            bg-black-1
            py-1
            px-2
            rounded-md
            text-base
          "
        >
          <input
            class="border-none bg-transparent outline-none"
            placeholder="Search"
            type="text"
            name=""
            id=""
            style="max-width: 150px"
          />
          <i class="bx bx-search"></i>
        </div>
        <div><i class="bx bx-at text-gray-400 hover:text-gray-300"></i></div>
        <div>
          <i class="bx bx-question-mark text-gray-400 hover:text-gray-300"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>
<template>
  <div class="grid grid-cols-6">
    <div
      class="col-span-1 flex items-start pt-1 h-screen justify-center font-sans text-2xl font-bold bg-[#2e8e84] text-white"
      style="font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;"
      >Sidebar content</div
      >
    <div class="col-span-5 h-screen bg-[#2e8e84]">
      <header class="flex items-center justify-start pl-6 h-[6vh] text-white font-medium">Header content</header>
      <div class="h-[94vh] w-[82.3vw] rounded-t-3xl rounded-b-none bg-gray-200 px-4 py-2">
        <slot/>
      </div>
    </div>

  </div>
</template>

<style>
header {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
</style>

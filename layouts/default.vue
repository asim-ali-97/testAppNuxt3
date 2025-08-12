<template>
  <div class="grid grid-cols-6">
    <Sidebar
      class="col-span-1 flex items-start pt-1 h-screen justify-center font-sans text-2xl font-bold bg-[#2e8e84] text-white"
      >Sidebar content</Sidebar
      >
    <div class="col-span-5 h-screen bg-[#2e8e84]">
      <header class="flex items-center justify-start pl-6 h-[6vh] text-white font-medium">Header content</header>
      <div class="h-[94vh] w-[82vw] rounded-3xl bg-gray-200 p-5">
        <slot/>
      </div>
    </div>

  </div>
</template>

<style>
Sidebar {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
header {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
</style>

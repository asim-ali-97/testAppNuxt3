<script setup>

const chkbxVal = ref(false);
const isRemember = computed(() => {
  if(chkbxVal.value){
    return "Yes"
  } else {
    return "No"
  }
});

definePageMeta({
  layout: "auth",
});
</script>

<template>
  <div
    class="flex items-center justify-center p-12 bg-white w-auto h-auto rounded-[5px]"
  >
    <div class="flex flex-col gap-3 p-[4px]">
      <div class="flex justify-center">
        <p class="text-3xl font-bold">Login</p>
      </div>
      <div class="flex flex-col gap-1">
        <label for="username">Username</label>
        <input
          type="text"
          id="username"
          placeholder="Enter your User-Name"
          class="border border-black rounded-md px-2 py-1 w-[20vw]"
        />
      </div>
      <div class="flex flex-col gap-1">
        <label for="password">Password</label>
        <input
          type="password"
          id="password"
          placeholder="Enter password"
          class="border border-black rounded-md px-2 py-1 w-[20vw]"
        />
      </div>
      <div class="flex items-center gap-4">
        <h3>Remember Me</h3>
        <input type="checkbox" v-model="chkbxVal" class="mt-[2px] size-4 cursor-pointer bg-black">
        <h2>{{ isRemember }}</h2>
      </div>
      <div class="flex items-end justify-end w-full">
        <NuxtLink to="/" class="cursor-pointer underline text-xs">Go to Home Page</NuxtLink>
      </div>
    </div>
  </div>
</template>

<style scoped>
p {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
</style>

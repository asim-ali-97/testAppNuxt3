<script setup>
const route = useRoute();
const data = ref([]);

data.value = await useFetch("https://fakestoreapi.com/users");
</script>
<template>
  <div class="flex items-center h-[40px]">
    <h1 class="text-xl font-bold">Home Page</h1>
  </div>

  <button
    class="w-auto py-2 px-6 rounded-lg bg-[#2e8e84] text-white text-[12px]"
  >
    <NuxtLink to="/product"> Go to Products page </NuxtLink>
  </button>
  <button
    class="w-auto py-2 px-6 rounded-lg bg-[#2e8e84] text-white text-[12px]"
  >
    <NuxtLink to="/user"> Go to Users page </NuxtLink>
    <!-- <NuxtLink to="/user/hello-world"> Go to Users page </NuxtLink> -->
  </button>
</template>

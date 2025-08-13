<script setup>
const route = useRoute();
const data = ref([]);
data.value = await useFetch("https://fakestoreapi.com/users");

onMounted(async () => {
  // data.value = await useFetch('https://fakestoreapi.com/users');
});

// onMounted(() => {
//   console.log("HERE IS IHE ROUTE::: ",route)
//   console.log(route.href)
// })
</script>

<template>
  <div class="flex items-center h-[40px]">
    <!-- <h1 class="text-xl font-bold">Products</h1> -->
     <h1 class="text-xl font-bold">User Page {{ route.params.id }}</h1>
  </div>
  <pre>{{ data?.data[1] }}</pre>
</template>

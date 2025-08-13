<script setup>
const route = useRoute();
const data = ref([]);
data.value = await useFetch("https://fakestoreapi.com/products");

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
    <h1 class="text-xl font-bold">Products</h1>
  </div>
  <div class="flex flex-wrap gap-12">
    <div v-for="product in data.data" class="">
      <h1>{{ product.price }}</h1>
      <!-- <img class="h-[200px]" :src="product.image" alt="" /> -->
    </div>
  </div>
  <!-- <pre>Total Products {{ data?.data }}</pre> -->
</template>

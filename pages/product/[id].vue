<script setup>
const route = useRoute();
const data = ref([]);
data.value = await useFetch('https://fakestoreapi.com/products')


onMounted(async () => {
  // data.value = await useFetch('https://fakestoreapi.com/users');
})



// onMounted(() => {
//   console.log("HERE IS IHE ROUTE::: ",route)
//   console.log(route.href)
// })


</script>


<template>
  <pre>{{ data?.data[1] }}</pre>
  <h1>Blog post {{ route.params.id }}</h1>
</template>

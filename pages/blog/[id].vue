<script setup>
const route = useRoute();
const data = ref([]);
data.value = await useFetch('https://api.agify.io?name=meelad')


onMounted(async () => {
  // data.value = await useFetch('https://api.agify.io?name=meelad');
})



// onMounted(() => {
//   console.log("HERE IS IHE ROUTE::: ",route)
//   console.log(route.href)
// })


</script>


<template>
  <pre>{{ data.data.count }}</pre>
  <h1>Blog post {{ route.params.id }}</h1>
</template>

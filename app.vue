<!-- <template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtWelcome />
  </div>
</template> -->


<!-- <template>
  <h1>Hello World!</h1>
</template> -->

<!-- <template>
  <NuxtPage />
</template> -->


<template>
  <NuxtLayout>
    <NuxtPage class="page" />
  </NuxtLayout>  
</template>

<style>
body{
  box-sizing: border-box;
}
.page{
  height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
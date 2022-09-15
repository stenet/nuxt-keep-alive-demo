<script lang="ts" setup>
const route = useRoute();
</script>

<template>
  <div>
    <h1>Product {{ route.params.id }}</h1>
    <input type="text">
    <ProductInfo/>
  </div>
</template>

<style scoped>

</style>
<script lang="ts" setup>
const route = useRoute();
</script>

<template>
  <div>
    <h1>Person {{ route.params.id }}</h1>
    <input type="text">
  </div>
</template>

<style scoped>

</style>
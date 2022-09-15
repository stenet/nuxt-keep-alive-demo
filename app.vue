<script setup lang="ts">
import type { KeepAliveProps } from "@vue/runtime-core";

const keepalive: KeepAliveProps = {
  max: 10,
  exclude: ["NoKeepAlive"]
};
</script>

<template>
  <div>
    <nav>
      <NuxtLink to="/">index</NuxtLink>
      <NuxtLink to="/products">Products</NuxtLink>
      <NuxtLink to="/products/1">Product 1</NuxtLink>
      <NuxtLink to="/products/2">Product 2</NuxtLink>
      <NuxtLink to="/products/3">Product 3</NuxtLink>
      <NuxtLink to="/people">People</NuxtLink>
      <NuxtLink to="/people/1">Person 1</NuxtLink>
      <NuxtLink to="/people/2">Person 2</NuxtLink>
      <NuxtLink to="/people/3">Person 3</NuxtLink>
      <NuxtLink to="/no-keep-alive">No keep alive</NuxtLink>
    </nav>
    
    <NuxtPage :keepalive="keepalive"></NuxtPage>
  </div>
</template>

<style>
nav {
  display: flex;
  gap: 1rem;
}
</style>
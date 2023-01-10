<template>
    <!-- <Home-Welcome /> -->
  <HomeWelcome />
  <!-- <Counter /> -->
  <!-- Dynamic Components  -->
  <component :is="Counter"/>
</template>
<script setup>
const Counter = resolveComponent("Counter")
</script>
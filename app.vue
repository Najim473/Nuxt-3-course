<template>
    <!-- <Home-Welcome /> -->
  <!-- <HomeWelcome /> -->
  <!-- <Counter /> -->
  <!-- Dynamic Components  -->
  <!-- <component :is="Counter"/> -->
  <button @click="toggle">Toggle</button>
  <component :is="myComponent"/>
</template>
<script setup>
// const Counter = resolveComponent("Counter")
const myComponent = ref(resolveComponent("Counter"));
function toggle (){
  console.log(myComponent.value)
  myComponent.value = resolveComponent("Home-Welcome")
}
</script>
<template>
  <!-- <Home-Welcome /> -->
  <!-- <HomeWelcome /> -->
  <!-- <Counter /> -->
  <!-- Dynamic Components  -->
  <!-- <component :is="Counter"/> -->
  <button @click="toggle">Toggle</button>
  <!-- way 01 -->
  <!-- <component :is="myComponent"/> -->
  <!-- way 02  -->
  <div v-if="myComponent === 'welcome'">
    <HomeWelcome />
  </div>
  <counter />
</template>
<script setup>
// const Counter = resolveComponent("Counter")
// Way 01
// const myComponent = ref(resolveComponent("Counter"));
// Way 02
const myComponent = ref("counter");
function toggle() {
  // Way 01
  // console.log(myComponent.value)
  // myComponent.value = resolveComponent("Home-Welcome")
  // Way 02
  myComponent.value = "welcome";
}
</script>

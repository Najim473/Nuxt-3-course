<template>
  <a :style="{ cursor: 'pointer' }" @click="view('home')">Home</a>
  <br />
  <br />
  <a :style="{ cursor: 'pointer' }" @click="view('counter')">Counter</a>
  <br />
  <br />
  <!-- <HomeWelcome v-if="page === 'home'" />
  <br />
  <br />
  <Counter v-if="page === 'counter'" /> -->
  <!-- It's will work when only need  -->
  <LazyHomeWelcome v-if="page === 'home'" />
  <br />
  <br />
  <LazyCounter v-if="page === 'counter'" />
</template>
<script setup>
const page = ref("home");
function view(name) {
  page.value = name;
}
</script>

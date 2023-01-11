<template>
    <h2>Hello index page</h2>
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="about">About</NuxtLink>
    <!-- By clicking redirect page  -->
    <button @click="moveToAbout">Take me to about page</button>
</template>
<script setup>
const moveToAbout =()=>{
    navigateTo("about")
}
</script>
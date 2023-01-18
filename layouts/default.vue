<template>
   <nav>
    <NuxtLink to="/">Home</NuxtLink>
  <br>
  <br>
  <NuxtLink to="about">About</NuxtLink>  
  <br>
  <br>
  <NuxtLink to="/profile">Profile</NuxtLink>
  <br>
  <br><br>
   </nav>
  <!-- Here nuxt will replace page content  -->
  <slot></slot>
</template>

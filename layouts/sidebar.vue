<template>
 <main class="user-layout">
  <article class="sidebar">
    <p>Dashboard</p>
    <p>Settings</p>
  </article>
  <section>
    <slot></slot>
  </section>
 </main>
</template>
<style>
.user-layout{
  display: flex;
  align-content: center;
  justify-content:space-evenly;
}
.sidebar {
  display: flex;
  flex-direction: column;
  font-size: 30px;
}
</style>

<script setup></script>

<template>
  <Header class="header"> </Header>
  <div class="wrapper">
    <aside class="aside"></aside>
    <main class="main">
      <router-view />
    </main>
  </div>
</template>

<style lang="css">
.header {
  background-color: hsla(212, 14%, 19%, 1);
  height: 36px;
  display: flex;
  align-items: center;
  gap: 8px;
}

.wrapper {
  display: flex;
  height: calc(100vh - 36px);
}

.aside {
  width: 13%;
  background-color: hsla(212, 14%, 19%, 1);
}

.main {
  width: 70%;
  background-color: hsla(0, 0%, 100%, 1);
}
</style>

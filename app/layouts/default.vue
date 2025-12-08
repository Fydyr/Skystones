<template>
  <div class="app-layout">
    <HeaderComponent />
    <main class="main-content">
      <slot />
    </main>
    <FooterComponent />
  </div>
</template>

<script setup lang="ts">
</script>

<style scoped>
.app-layout {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  background: linear-gradient(rgba(22, 33, 62, 0.9), rgba(22, 33, 62, 0.9)),
              url('/placeholder-background.jpg') center/cover no-repeat fixed;
  background-color: #16213e;
}

.main-content {
  flex: 1;
}
</style>

<template>
  <header class="header">
    <div class="header-container">
      <div class="logo">
        <a href="/">
          <h1>Aeroliths</h1>
        </a>
      </div>

      <button class="mobile-menu-btn" @click="mobileMenuOpen = !mobileMenuOpen" aria-label="Toggle menu">
        <span v-if="!mobileMenuOpen">☰</span>
        <span v-else>✕</span>
      </button>

      <nav class="nav" :class="{ 'nav-open': mobileMenuOpen }">
        <a href="/" @click="mobileMenuOpen = false">Home</a>
        <a href="/play" @click="mobileMenuOpen = false">Play</a>
        <a href="/rules" @click="mobileMenuOpen = false">Rules</a>
        <a href="/leaderboard" @click="mobileMenuOpen = false">Leaderboard</a>
      </nav>
    </div>
  </header>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const mobileMenuOpen = ref(false)
</script>

<style scoped src="~/assets/css/header.css"></style>

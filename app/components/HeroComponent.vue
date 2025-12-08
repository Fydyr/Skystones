<template>
  <div class="game-intro">
    <!-- Hero Section -->
    <section class="hero-section">
      <div class="hero-content">
        <h1 class="hero-title">Welcome to Aeroliths</h1>
        <p class="hero-subtitle">
          Discover the legendary strategy game inspired by Skylanders Skystones
        </p>
        <div class="hero-image-placeholder">
          <span class="placeholder-text">[Hero Image - Game Board]</span>
        </div>
      </div>
    </section>

    <!-- Game Rules Section -->
    <section class="rules-section">
      <h2 class="section-title">How to Play?</h2>

      <div class="rules-grid">
        <UCard class="rule-card">
          <template #header>
            <div class="card-header">
              <UIcon name="i-heroicons-squares-2x2" class="card-icon" />
              <h3>The Board</h3>
            </div>
          </template>
          <p>
            Face your opponent on a 3x3 grid. Each player strategically places
            their stones to conquer the enemy territory.
          </p>
          <div class="image-placeholder">
            <span class="placeholder-text">[Image - 3x3 Board]</span>
          </div>
        </UCard>

        <UCard class="rule-card">
          <template #header>
            <div class="card-header">
              <UIcon name="i-heroicons-cube" class="card-icon" />
              <h3>The Stones</h3>
            </div>
          </template>
          <p>
            Each stone has values on its 4 sides (top, bottom, left, right).
            The higher the value, the more powerful it is in that direction!
          </p>
          <div class="image-placeholder">
            <span class="placeholder-text">[Image - Stone with values example]</span>
          </div>
        </UCard>

        <UCard class="rule-card">
          <template #header>
            <div class="card-header">
              <UIcon name="i-heroicons-arrow-path" class="card-icon" />
              <h3>The Conquest</h3>
            </div>
          </template>
          <p>
            When you place a stone, compare its values with adjacent stones.
            If your value is higher, you capture the opponent's stone!
          </p>
          <div class="image-placeholder">
            <span class="placeholder-text">[Image - Capture example]</span>
          </div>
        </UCard>

        <UCard class="rule-card">
          <template #header>
            <div class="card-header">
              <UIcon name="i-heroicons-trophy" class="card-icon" />
              <h3>Victory</h3>
            </div>
          </template>
          <p>
            The player who controls the most stones at the end of the game wins.
            Strategy and anticipation are the keys to success!
          </p>
          <div class="image-placeholder">
            <span class="placeholder-text">[Image - Victory board]</span>
          </div>
        </UCard>
      </div>
    </section>

    <!-- Strategy Tips Section -->
    <section class="tips-section">
      <h2 class="section-title">Strategic Tips</h2>

      <div class="tips-container">
        <UAlert
          icon="i-heroicons-light-bulb"
          color="primary"
          variant="soft"
          title="Control the center"
          description="The center of the board is crucial! A well-placed stone in the center can influence up to 4 other squares."
        />

        <UAlert
          icon="i-heroicons-chart-bar"
          color="warning"
          variant="soft"
          title="Balance your stones"
          description="Don't put all your eggs in one basket with ultra-powerful stones on one side and weak on the other. Balance is key!"
        />

        <UAlert
          icon="i-heroicons-eye"
          color="success"
          variant="subtle"
          title="Think ahead"
          description="Always think one move ahead. Which square will your opponent target next?"
        />
      </div>
    </section>

    <!-- CTA Section -->
    <section class="cta-section">
      <div class="cta-content">
        <h2 class="cta-title">Ready to become an Aeroliths master?</h2>
        <p class="cta-text">
          Challenge players from around the world, collect legendary stones,
          and climb the leaderboard!
        </p>
        <div class="cta-buttons">
          <UButton size="xl" color="primary">
            Start Playing
          </UButton>
          <UButton size="xl" color="secondary" variant="outline">
            Learn More
          </UButton>
        </div>
        <div class="cta-image-placeholder">
          <span class="placeholder-text">[Image - Stone collection]</span>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup lang="ts">
</script>

<style scoped src="~/assets/css/hero.css"></style>

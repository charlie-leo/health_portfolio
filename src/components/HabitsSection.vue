<template>
  <section class="habits-section">
    <div class="habits-left">
      <h2>Are Your Habits<br />Helping or Hurting?</h2>
    </div>
    <div class="habits-right">
      <nav>
        <a href="https://docs.google.com/forms/d/e/1FAIpQLSduFuEQwbU2DMc626VeJUdqoy_BKnw6Q2y7nDMH_APHFtqfIQ/viewform?usp=header" target="_blank" rel="noopener noreferrer">
          <span class="italic">Are <b>your</b> Habits Helping or Hurting?</span>
          <span class="arrow">&rarr;</span>
        </a>
      </nav>
    </div>
  </section>
</template>

<script setup lang="ts">
</script>

<style scoped>
.habits-section {
  display: flex;
  background: #4e7575;
  color: #fff;
  padding: 2.5rem 2rem;
  align-items: center;
  justify-content: space-between;
  border-radius: 0 0 12px 12px;
  margin-bottom: 2rem;
}

.habits-left h2 {
  font-size: 2rem;
  font-weight: 500;
  margin: 0;
}

.habits-right {
  font-size: 1.2rem;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.italic {
  font-style: italic;
}

.arrow {
  font-size: 1.5rem;
  margin-left: 0.5rem;
}

@media (max-width: 900px) {
  .habits-section {
    flex-direction: column;
    gap: 1.5rem;
    text-align: center;
  }
}
</style>

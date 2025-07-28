<template>
  <section class="story-section" id="stories">
    <h2>Stories</h2>
    <div class="story-cards">
      <div class="story-card">
        <h3>Struggling with Diet and Stress</h3>
        <p>
          When Priya moved to Canada for studies, she found it difficult to cook and started eating instant noodles and fast food daily. She began feeling tired, gained weight, and noticed she couldn’t focus in class. After visiting the campus health center, she learned about meal planning and joined a student cooking club. With better eating habits and regular walking, her mood and energy improved, and her academic performance increased.
        </p>
      </div>
      <div class="story-card highlight">
        <h3>Physical Activity and Mental Health</h3>
        <p>
          Ahmed spent most of his time studying and working part-time. He rarely exercised due to cold weather and long hours. Over time, he felt isolated and anxious. A friend encouraged him to join a free campus gym class. Regular workouts and meeting new friends helped him feel less lonely, reduced his anxiety, and gave him better sleep.
        </p>
      </div>
      <div class="story-card">
        <h3>Coping Without Substance Use</h3>
        <p>
          Mei felt overwhelmed with assignments and part-time work. Some classmates used alcohol to relax, but Mei joined a student support group instead. Talking to peers and learning stress management techniques helped her manage pressure without turning to substances. Today, she mentors new students facing similar challenges.
        </p>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
</script>

<style scoped>
.story-section {
  display: flex;
  color: #4e7575;
  padding: 2.5rem 2rem;
  flex-direction: column;
  align-items: start;
  justify-content: space-between;
  border-radius: 12px;
  margin-bottom: 2rem;
}
.story-section h2 {
  font-size: 2rem;
  margin-bottom: 2rem;
  color: #3a4a4a;
}
.story-cards {
  display: flex;
  flex-direction: column;
  width: 100%;
  gap: 1.5rem;
  flex-wrap: nowrap;
  justify-content: center;
}
.story-card {
  background: #e0ede7;
  border-radius: 12px;
  padding: 1.5rem 1.2rem;
  width: 100%;
  text-align: center;
  color: #3a4a4a;
  box-shadow: 0 2px 8px rgba(60, 60, 60, 0.04);
}
.story-card.highlight {
  background: #fff;
  border: 2px solid #b7d3c6;
}

.story-card h3 {
  font-weight: bold;
  text-align: start;
  margin-bottom: 8px;
}
.story-card p {
  font-size: 14px;
  padding-left: 0;
  text-align: left;
}

@media (max-width: 900px) {
  .story-cards {
    flex-direction: column;
    align-items: center;
  }
}
</style>

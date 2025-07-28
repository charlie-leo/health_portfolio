<template>
  <section class="story-section" id="tips">
    <h2>Tips & Solutions</h2>
    <div class="story-cards">
      <div class="story-card">
        <h3>Healthy Habits</h3>
        <ul>
          <li>Meal planning for the week (with examples of affordable meals).</li>
          <li>Building a balanced plate (protein, carbs, veggies).</li>
          <li>Exercise routines for students with busy schedules.</li>
          <li>How to set achievable health goals.</li>
        </ul>
      </div>
      <div class="story-card highlight">
        <h3>Stress Management</h3>
        <ul>
          <li>Mindfulness exercises and breathing techniques.</li>
          <li>Managing time effectively to balance studies, work, and rest.</li>
          <li>Journaling and other positive coping strategies.</li>
        </ul>
      </div>
      <div class="story-card">
        <h3>Getting Help</h3>
        <ul>
          <li>Steps to contact university counselors or mental health professionals.</li>
          <li>Peer support networks and cultural student groups.</li>
          <li>Contact numbers for crisis helplines.</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
</script>

<style scoped>
.story-section {
  display: flex;
  background: #4e7575;
  color: #fff;
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
  color: #fff;
}
.story-cards {
  display: flex;
  flex-direction: row;
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
  text-align: center;
}
.story-card ul li {
  font-size: 14px;
  padding-left: 0px;
  text-align: left;
}


.resource-btn {
  margin-top: 1rem;
  background: #4e7575;
  color: #fff;
  border: none;
  border-radius: 6px;
  padding: 0.5rem 1.2rem;
  font-size: 1rem;
  cursor: pointer;
  transition: background 0.2s;
}
.resource-btn:hover {
  background: #7bb7b7;
}
@media (max-width: 900px) {
  .story-cards {
    flex-direction: column;
    align-items: center;
  }
}
</style>

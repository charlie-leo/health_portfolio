<template>
  <section class="findings-section" id="research">
    <h2>Research Section</h2>
    <div class="findings-cards">
      <div class="finding-card">
        <div class="icon">🌱</div>
        <h3>Diet & Nutrition Change</h3>
        <h4>Struggles </h4>
        <ul>
          <li>Difficulty finding familiar food items.</li>
          <li>High cost of fresh fruits and vegetables.</li>
          <li>Limited time for cooking due to studies.</li>
        </ul>
        <h4>Impacts</h4>
        <ul>
          <li>Nutrient deficiencies affecting concentration and energy.</li>
          <li>Over-reliance on processed/fast food leading to weight changes.</li>
        </ul>
        <h4>Additional Subtopics</h4>
        <ul>
          <li>Importance of hydration.</li>
          <li>Cultural differences in meal patterns (e.g., skipping breakfast).</li>
          <li>Tips for grocery shopping on a budget.</li>
        </ul>
      </div>
      <div class="finding-card">
        <div class="icon">🍎</div>
        <h3>Physical Health & Lifestyle</h3>
        <h4>Challenges</h4>
        <ul>
          <li>Busy academic schedules reduce time for exercise.</li>
          <li>Weather conditions (cold climate discourages outdoor activities).</li>
          <li>Lack of awareness about free campus facilities.</li>
        </ul>
        <h4>Impacts</h4>
        <ul>
          <li>Weaker immune system and increased fatigue.</li>
          <li>Higher risk of obesity and lifestyle-related diseases.</li>
        </ul>
        <h4>Additional Subtopics</h4>
        <ul>
          <li>Role of sleep in physical and mental health.</li>
          <li>Easy home workouts for students.</li>
          <li>How physical activity helps build social connections.</li>
        </ul>

      </div>
      <div class="finding-card highlight">
        <div class="icon">💚</div>
        <h3>Mental Health & Stress</h3>
        <h4>Challenges</h4>
        <ul>
          <li>Cultural shock, language barriers, and homesickness.</li>
          <li>Academic pressure, visa stress, and part-time job responsibilities.</li>
        </ul>
        <h4>Impacts</h4>
        <ul>
          <li>Anxiety, depression, social isolation.</li>
          <li>Poor academic performance and burnout.</li>
        </ul>
        <h4>Additional Subtopics</h4>
        <ul>
          <li>Benefits of mindfulness and meditation.</li>
          <li>How social support systems (friends, clubs) help mental health.</li>
          <li>Importance of asking for professional help early.</li>
        </ul>
      </div>
      <div class="finding-card">
        <div class="icon">🧪</div>
        <h3>Substance Use</h3>
        <h4>Reasons for Use</h4>
        <ul>
          <li>Peer pressure, loneliness, or coping with academic stress.</li>
          <li>Easy access to alcohol and recreational drugs in some countries.</li>
        </ul>
        <h4>Risks</h4>
        <ul>
          <li>Addiction, health problems, academic failures.</li>
        </ul>
        <h4>Additional Subtopics</h4>
        <ul>
          <li>Myths vs. facts about substance use.</li>
          <li>How cultural differences affect attitudes toward alcohol and drugs.</li>
          <li>Resources for substance use prevention and recovery.</li>
        </ul>

      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
</script>

<style scoped>
.findings-section {
  background: #f5f6ef;
  padding: 2.5rem 1.5rem 2rem 1.5rem;
}
.findings-section h2 {
  font-size: 2rem;
  margin-bottom: 2rem;
  color: #3a4a4a;
}
.findings-cards {
  display: flex;
  flex-direction: row;
  gap: 1.5rem;
  flex-wrap: wrap;
  justify-content: space-around;
}
.finding-card {
  background: #b7d3c6;
  border-radius: 12px;
  padding: 1.5rem 1.2rem;
  width: 47%;
  text-align: center;
  color: #3a4a4a;
  box-shadow: 0 2px 8px rgba(60, 60, 60, 0.04);
}
.finding-card .icon {
  font-size: 2rem;
  margin-bottom: 0.7rem;
}
.finding-card.highlight {
  background: #ede7c6;
}
.finding-card h3 {
  font-weight: bold;

}
.finding-card h4 {
  font-weight: bold;
  align-self: start;
  text-align: start;
}
.finding-card ul li {
  font-size: 14px;
  padding-left: 0px;
  text-align: left;
}
@media (max-width: 900px) {
  .findings-cards {
    flex-direction: column;
    align-items: center;
  }
}
</style>

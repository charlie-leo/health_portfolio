<template>
  <section class="hero-section" id="home">
    <div class="hero-left">
      <div style="font-weight: bold">
        <span>Link Between</span>
        <br>
        <span
          style="font-size: 36px; font-weight: bold; line-height: 36px"
        >Diet, Physical & Mental Health, and Substance Use</span>
        <br>
        <span>in International Students</span>
      </div>
      <br>
      <p class="subtitle">Supporting International Students for a Healthier Future</p>
      <H3 style="font-weight: bold">About the Project</H3>
      <p style="font-style: italic">To spread awareness about how lifestyle changes affect international students’ health.</p>
      <p style="font-style: italic">To provide practical tips, resources, and real experiences to help students adapt better.</p>
<!--      <button class="hero-btn">Explore the Journey</button>-->
    </div>
    <div class="hero-right">
      <h2>About US</h2>
      <div class="about-block">
        <h3>Team Members</h3>
        <ul>
          <li>Akshita Vig</li>
          <li>Kritika Rana</li>
        </ul>
        <h3>Project Goal</h3>
        <ul>
          <li>To research and present the connection between diet, physical health, mental health, and substance use among international students.</li>
        </ul>
        <h3>Why This Topic Matters</h3>
        <ul>
          <li>International students face cultural and environmental changes that affect their well-being.</li>
          <li>Raising awareness can help students make better lifestyle choices and seek support when needed.</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
</script>

<style scoped>
.hero-section {
  display: flex;
  background: #e0ede7;
  padding: 3rem 2rem 2rem 2rem;
  border-radius: 0 0 12px 12px;
  gap: 2rem;
}
.hero-left {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  color: #3a4a4a;
  padding: 2rem 1rem 2rem 2rem;
}
.hero-left h1 {
  font-size: 2.5rem;
  font-weight: 700;
  /* color: #f5f6ef; */
  margin-bottom: 1rem;
  line-height: 1.1;
}
.subtitle {
  /* color: #f5f6ef; */
  font-size: 1.1rem;
  margin-bottom: 2rem;
}
.hero-btn {
  background: #3a4a4a;
  color: #fff;
  border: none;
  border-radius: 6px;
  padding: 0.7rem 1.5rem;
  font-size: 1rem;
  cursor: pointer;
  transition: background 0.2s;
}
.hero-btn:hover {
  background: #7bb7b7;
}
.hero-right {
  flex: 1;
  background: #f5f6ef;
  border-radius: 12px;
  padding: 2rem 2rem 2rem 1rem;
  color: #3a4a4a;
}
.hero-right h2 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
}
.about-block h3 {
  margin-top: 1.2rem;
  margin-bottom: 0.5rem;
  font-size: 1.1rem;
  color: #6b7c7c;
}
.about-block ul {
  margin: 0 0 0.5rem 1.2rem;
  padding: 0;
  list-style: disc;
}
.about-block p {
  margin: 0.5rem 0 0 0;
}
@media (max-width: 900px) {
  .hero-section {
    flex-direction: column;
    padding: 2rem 1rem;
  }
  .hero-left, .hero-right {
    padding: 1rem;
  }
}
</style>

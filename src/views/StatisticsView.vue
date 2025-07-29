<template>
  <div style="height: 100vh"  >
    <HeaderSection />
    <section class="stats-section">
      <h2>Statistics & Facts</h2>
      <p class="intro">
        Here are some key statistics about the health and well-being of international students,
        based on research studies and surveys.
      </p>

      <div class="stats-grid">
        <div class="stat-card">
          <h3>Mental Health Issues</h3>
          <p>
            In South Korea during COVID, <b>47.1%</b> reported sleep problems, <b>39.6%</b> reported
            anxiety, and <b>49%</b> reported depression.
          </p>
        </div>

        <div class="stat-card">
          <h3>Food Insecurity</h3>
          <p>
            In US colleges, roughly <b>43.5%</b> of students face food insecurity— double the
            general population rate.
          </p>
        </div>

        <div class="stat-card">
          <h3>Dietary Improvements</h3>
          <p>
            Reducing high-calorie foods → <b>7.5%</b> health improvement. Increasing fiber intake →
            <b>+5.68%</b> benefit.
          </p>
        </div>

        <div class="stat-card">
          <h3>Substance Use & Mental Illness</h3>
          <p>
            Over <b>15%</b> with substance use disorder have a co-occurring mental illness. Those
            with mental illness are up to <b>3x</b> more likely to have substance issues.
          </p>
        </div>
      </div>

      <h3 class="chart-title">Visual Representation</h3>
      <div class="charts-container">
        <div>
          <canvas id="mentalChart"></canvas>
        </div>
        <div>
          <canvas id="foodChart"></canvas>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup lang="ts">
import { onMounted } from 'vue'
import Chart from 'chart.js/auto'
import HeaderSection from '@/components/HeaderSection.vue'

onMounted(() => {
  // Bar Chart for Mental Health Issues
  new Chart(document.getElementById('mentalChart') as HTMLCanvasElement, {
    type: 'bar',
    data: {
      labels: ['Sleep Problems', 'Anxiety', 'Depression'],
      datasets: [
        {
          label: '% of Students',
          data: [47.1, 39.6, 49],
          backgroundColor: ['#6db6b6', '#4e7575', '#355b5b'],
        },
      ],
    },
    options: {
      responsive: true,
      plugins: { legend: { display: false } },
    },
  })

  // Pie Chart for Food Insecurity
  new Chart(document.getElementById('foodChart') as HTMLCanvasElement, {
    type: 'pie',
    data: {
      labels: ['Food Insecure', 'Food Secure'],
      datasets: [
        {
          data: [43.5, 56.5],
          backgroundColor: ['#4e7575', '#e0ede7'],
        },
      ],
    },
    options: { responsive: true },
  })
})
</script>

<style scoped>
.stats-section {
  background: #f5f6ef;
  color: #4e7575;
  padding: 2.5rem 1.5rem;
  border-radius: 0 0 12px 12px;
}

.stats-section h2 {
  font-size: 2rem;
  text-align: center;
  margin-bottom: 1rem;
}

.intro {
  text-align: center;
  max-width: 700px;
  margin: 0 auto 2rem;
  font-size: 1rem;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 1.5rem;
  margin-bottom: 2rem;
}

.stat-card {
  background: #fff;
  color: #3a4a4a;
  padding: 1rem;
  border-radius: 10px;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.15);
}

.stat-card h3 {
  margin-bottom: 0.5rem;
  font-size: 1.2rem;
  color: #2c3e3e;
}

.chart-title {
  text-align: center;
  margin-bottom: 1rem;
  font-size: 1.5rem;
}

.charts-container {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  gap: 2rem;
}

.charts-container div {
  width: 100%;
}

canvas {
  background: #fff;
  padding: 10px;
  border-radius: 8px;
  height: 400px;
}
</style>

<template>
  <div style="height: 100vh"  >
    <HeaderSection />
  <section class="minutes-section">
    <h2>Meeting Minutes – Project: The Link Between Diet, Physical Health, Mental Health & Substance Use</h2>

    <p class="intro">
      This page documents all important meetings, discussions, and progress updates made by
      <b>Akshita Vig</b> and <b>Kritika Rana</b> while working on this research and website project.
    </p>

    <h3>Project Slogan</h3>
    <p class="slogan">We Can Do It! Two Minds – One Vision</p>

    <h3>Meeting Records</h3>
    <table class="minutes-table">
      <thead>
      <tr>
        <th>Date</th>
        <th>Topic</th>
        <th>Presenter</th>
        <th>Action Items / Remarks</th>
        <th>Status</th>
      </tr>
      </thead>
      <tbody>
      <tr>
        <td>20–21 June</td>
        <td>Topic Discussion</td>
        <td>Both</td>
        <td>Finalized topic, understanding the topic on a broader perspective</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>25 June</td>
        <td>Project Planning</td>
        <td>Both</td>
        <td>Outlined overall project plan</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>29 June</td>
        <td>Task Division</td>
        <td>Both</td>
        <td>Divided tasks according to strengths and weaknesses</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>01 July</td>
        <td>Website Outline & Structure</td>
        <td>Kritika</td>
        <td>Wireframe & section breakdown discussion</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>05 July</td>
        <td>Topics to Cover</td>
        <td>Akshita</td>
        <td>Initial drafting of basic content</td>
        <td>80% Completed</td>
      </tr>
      <tr>
        <td>06 July</td>
        <td>Stories/Incidents</td>
        <td>Akshita</td>
        <td>Gathered real incidents and case studies to enhance content</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>08 July</td>
        <td>Logo Design, Color & Formatting</td>
        <td>Kritika</td>
        <td>Logo drafts, theme finalization</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>10 July</td>
        <td>Logo Design, Color & Formatting</td>
        <td>Kritika</td>
        <td>Logo drafts, theme finalization</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>13 July</td>
        <td>Information gathering and content for website</td>
        <td>Akshita</td>
        <td>Content for website</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>17 July</td>
        <td>Home screen and sections</td>
        <td>Kritika</td>
        <td>Design the homescreen and sections</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>20 July</td>
        <td>Statistics Content and screen</td>
        <td>Akshita</td>
        <td>Added Chart to visualize the data.</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>20 July</td>
        <td>Research about the Food and Recipes and add the details in websites</td>
        <td>Kritika</td>
        <td>Added common meals, Everyday Meal, Added helping websites link</td>
        <td>50% Completed</td>
      </tr>
      <tr>
        <td>24 July</td>
        <td>Research about the Food and Recipes and add the details in websites</td>
        <td>Kritika</td>
        <td>Added common meals, Everyday Meal, Added helping websites link</td>
        <td>100% Completed</td>
      </tr>
      <tr>
        <td>27 July</td>
        <td>Added the Records to the website</td>
        <td>Akshita</td>
        <td>Record section in the website</td>
        <td>Completed</td>
      </tr>
      <tr>
        <td>27 July</td>
        <td>Take habit survey using google form and collect the data in the excel sheet.</td>
        <td>Kritika</td>
        <td>Google form, Link Excel sheet</td>
        <td>100% Completed</td>
      </tr>
      </tbody>
    </table>

    <h3>Related Project Pages</h3>
    <ul class="links-list">
      <li><router-link to="/">Home</router-link></li>
      <li><router-link to="/statistics">Statistics & Facts</router-link></li>
      <li><router-link to="/recipes">Healthy Recipes & Diet Plans</router-link></li>
      <li><router-link to="/questions">Self-Assessment Quiz</router-link></li>
    </ul>
  </section>
  </div>
</template>

<script setup lang="ts">
import HeaderSection from '@/components/HeaderSection.vue'
</script>

<style scoped>
.minutes-section {
  background: #f5f6ef;
  color: #3a4a4a;
  padding: 2.5rem 1.5rem;
  border-radius: 0 0 12px 12px;
}

.minutes-section h2 {
  font-size: 2rem;
  text-align: center;
  margin-bottom: 1rem;
}

.intro {
  text-align: center;
  max-width: 750px;
  margin: 0 auto 2rem;
  font-size: 1rem;
}

.slogan {
  text-align: center;
  font-size: 1.2rem;
  font-weight: bold;
  margin-bottom: 1.5rem;
}

.minutes-table {
  width: 100%;
  border-collapse: collapse;
  margin-bottom: 2rem;
}

.minutes-table th,
.minutes-table td {
  border:1px solid rgba(158, 175, 175, 0.58);
  padding: 8px;
  text-align: center;
}

.minutes-table th {
  color: #f5f6ef;
  background: #3a5b5b;
}

.links-list {
  list-style: none;
  padding-left: 0;
  text-align: start;
}

.links-list li {
  margin: 0.4rem 0;
}

.links-list a {
  color: #348c12;
  text-decoration: none;
}

.links-list a:hover {
  text-decoration: underline;
}
</style>

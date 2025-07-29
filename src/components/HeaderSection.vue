<template>
  <nav class="header-nav">
    <div class="logo">DPMHS</div>
    <ul>
      <li>
        <router-link :to="{ path: '/', hash: '#home' }">Home</router-link>
      </li>
      <li>
        <router-link :to="{ path: '/', hash: '#research' }">Research</router-link>
      </li>
      <li>
        <router-link to="/statistics">Statistics</router-link>
      </li>
      <li>
        <router-link to="/recipes">Recipes</router-link>
      </li>
      <li>
        <router-link to="/records">Records</router-link>
      </li>
      <li>
        <router-link :to="{ path: '/', hash: '#tips' }">Tips & Resources</router-link>
      </li>
      <li>
        <router-link :to="{ path: '/', hash: '#stories' }">Stories</router-link>
      </li>
      <li>
        <router-link :to="{ path: '/', hash: '#contact' }">Contact</router-link>
      </li>
    </ul>
  </nav>
</template>

<script setup lang="ts">
</script>

<style scoped>
.header-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1.5rem 2rem 1.5rem 0;
  background: #f5f6ef;
  font-size: 1.1rem;
  border-bottom: 1px solid #e0e0d1;
}
.logo {
  font-weight: bold;
  font-size: 1.2rem;
  letter-spacing: 0.1em;
  color: #6b7c7c;
}
ul {
  display: flex;
  gap: 1.5rem;
  list-style: none;
  margin: 0;
  padding: 0;
}
ul li a {
  color: #3a4a4a;
  text-decoration: none;
  transition: color 0.2s;
}
ul li a:hover {
  color: #7bb7b7;
}
</style>

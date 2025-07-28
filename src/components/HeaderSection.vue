<template>
  <nav class="header-nav">
    <div class="logo">DPMHS</div>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#research">Research</a></li>
      <li><a href="#tips">Tips & Resources</a></li>
      <li><a href="#stories">Stories</a></li>
      <li><a href="#contact">Contact</a></li>
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

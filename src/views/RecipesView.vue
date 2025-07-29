<template>
  <div style="height: 100vh"  >
    <HeaderSection />
  <section class="recipes-section">
    <h2>Healthy Recipes & Diet Plans</h2>
    <p class="intro">
      International students often face challenges in eating healthy due to budget, time, and cultural changes.
      Maintaining a balanced diet can improve mood, energy, and academic performance.
    </p>

    <h3>Daily Meal Ideas on a Budget</h3>
    <div class="recipes-grid">
      <div class="recipe-card">
        <h4>Breakfast</h4>
        <ul>
          <li>Overnight oats with fruit & nuts</li>
          <li><a href="https://www.eatingwell.com/gallery/13694/easy-cheap-healthy-college-meals/" target="_blank">Blueberry-Pecan Overnight Oatmeal</a></li>
        </ul>
      </div>

      <div class="recipe-card">
        <h4>Lunch</h4>
        <ul>
          <li>Vegetarian rice bowl with beans/tofu</li>
          <li><a href="https://www.theguardian.com/food/2022/jul/17/soy-chicken-wing-noodles-rice-bowls-banh-mi-uyen-luu-budget-vietnamese-recipes" target="_blank">Vietnamese-style Rice Bowl</a></li>
        </ul>
      </div>

      <div class="recipe-card">
        <h4>Dinner</h4>
        <ul>
          <li>One-pot lentil curry with vegetables</li>
          <li><a href="https://www.thespruceeats.com/16-cheap-low-fat-meals-4846254" target="_blank">Budget Low-Fat Meals</a></li>
        </ul>
      </div>

      <div class="recipe-card">
        <h4>Snacks</h4>
        <ul>
          <li>Greek yogurt with honey & fruit</li>
          <li>Popcorn with olive oil</li>
          <li>Carrot or celery sticks</li>
        </ul>
      </div>
    </div>

    <h3>Key Nutrients for Health</h3>
    <ul class="tips-list">
      <li>Leafy greens, B vitamins, Omega-3 foods support brain health.</li>
      <li>Whole grains, legumes, and fermented foods improve gut health.</li>
      <li>Hydration: 2–3 liters of water per day is essential for focus and mood.</li>
    </ul>

    <h3>Sample Weekly Meal Plan</h3>
    <table class="meal-table">
      <thead>
      <tr>
        <th>Day</th>
        <th>Breakfast</th>
        <th>Lunch</th>
        <th>Dinner</th>
        <th>Snack</th>
      </tr>
      </thead>
      <tbody>
      <tr>
        <td>Mon</td>
        <td>Overnight oats</td>
        <td>Veggie rice bowl</td>
        <td>Lentil curry & rice</td>
        <td>Popcorn or nuts</td>
      </tr>
      <tr>
        <td>Tue</td>
        <td>Yogurt + fruit</td>
        <td>Chickpea wrap</td>
        <td>Vegetable stir-fry</td>
        <td>Carrot sticks</td>
      </tr>
      <tr>
        <td>Wed</td>
        <td>Smoothie</td>
        <td>Tuna/tofu rice bowl</td>
        <td>Barley-lentil soup</td>
        <td>Greek yogurt</td>
      </tr>
      <tr>
        <td>Thu</td>
        <td>Whole wheat pancakes</td>
        <td>Leftover curry</td>
        <td>Tofu scramble & rice</td>
        <td>Fruit & yogurt</td>
      </tr>
      <tr>
        <td>Fri</td>
        <td>Oatmeal with berries</td>
        <td>Veggie pasta salad</td>
        <td>Baked tofu & veggies</td>
        <td>Hummus + veggies</td>
      </tr>
      </tbody>
    </table>

    <h3>More Recipe Resources</h3>
    <ul class="links-list">
      <li><a href="https://www.bbcgoodfood.com/recipes/collection/healthy-student-recipes" target="_blank">BBC Good Food – Healthy Student Recipes</a></li>
      <li><a href="https://www.thespruceeats.com/16-cheap-low-fat-meals-4846254" target="_blank">The Spruce Eats – Budget Low-Fat Meals</a></li>
      <li><a href="https://www.eatingwell.com/gallery/13694/easy-cheap-healthy-college-meals/" target="_blank">EatingWell – Easy, Cheap & Healthy Meals</a></li>
    </ul>
  </section>
  </div>
</template>

<script setup lang="ts">
import HeaderSection from '@/components/HeaderSection.vue'
</script>

<style scoped>
.recipes-section {
  background: #f5f6ef;
  color: #3a4a4a;
  padding: 2.5rem 1.5rem;
  border-radius: 0 0 12px 12px;
}

.recipes-section h2 {
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

h3 {
  margin-top: 2rem;
  margin-bottom: 0.8rem;
  font-size: 1.4rem;
  border-bottom: 1px solid rgba(158, 175, 175, 0.58);
  padding-bottom: 0.3rem;
}

.recipes-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.2rem;
  margin-bottom: 2rem;
}

.recipe-card {
  background: #4e7575;
  color: #e0ede7;
  padding: 1rem;
  border-radius: 10px;
}

.recipe-card h4 {
  margin-bottom: 0.5rem;
  color: #e0ede7;
}

.recipe-card ul {
  padding-left: 1rem;
}

.tips-list {
  padding-left: 1.2rem;
  margin-bottom: 1.5rem;
}

.meal-table {
  width: 100%;
  border-collapse: collapse;
  margin-bottom: 2rem;
}

.meal-table th,
.meal-table td {
  border: 1px solid rgba(158, 175, 175, 0.58);
  padding: 8px;
  text-align: center;
}

.links-list {
  padding-left: 1.2rem;
}

.links-list a {
  color: #41d81f;
  text-decoration: none;
}

.links-list a:hover {
  text-decoration: underline;
}
</style>

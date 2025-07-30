<template>
  <div class="quiz-section">
    <h1 class="habit-title">Are Your Habits Helping or Hurting?</h1>
    <p class="intro">
      Answer the following questions honestly to assess your lifestyle habits and get tips to improve your health.
    </p>

    <div class="questions-container">
      <QuestionCard
        v-for="(q, index) in questions"
        :key="index"
        :question="q"
        v-model="answers[index]"
      />
    </div>

    <button class="submit-btn" @click="submitQuiz">Submit Quiz</button>

    <div v-if="resultMessage" class="result-box">
      <h2>📊 Result</h2>
      <p>{{ resultMessage }}</p>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import QuestionCard from './QuestionCard.vue'

const questions = ref([
  {
    text: 'How many home-cooked meals do you eat per week?',
    options: [
      { label: '0–1', value: 0 },
      { label: '2–4', value: 1 },
      { label: '5–7', value: 2 },
    ],
  },
  {
    text: 'Do you often skip meals due to stress or lack of time?',
    options: [
      { label: 'Yes', value: 0 },
      { label: 'No', value: 2 },
    ],
  },
  {
    text: 'Do you exercise for at least 30 minutes, 3+ times per week?',
    options: [
      { label: 'Never', value: 0 },
      { label: '1–2 times', value: 1 },
      { label: '3+ times', value: 2 },
    ],
  },
  {
    text: 'How many hours of quality sleep do you get per night?',
    options: [
      { label: 'Less than 5 hours', value: 0 },
      { label: '5–7 hours', value: 1 },
      { label: '7+ hours', value: 2 },
    ],
  },
  {
    text: 'Do you consume alcohol or drugs to cope with stress?',
    options: [
      { label: 'Yes', value: 0 },
      { label: 'Sometimes', value: 1 },
      { label: 'No', value: 2 },
    ],
  },
  {
    text: 'How often do you feel lonely or homesick?',
    options: [
      { label: 'Often', value: 0 },
      { label: 'Sometimes', value: 1 },
      { label: 'Rarely', value: 2 },
    ],
  },
  {
    text: 'How often do you eat fruits and vegetables in a day?',
    options: [
      { label: 'Rarely', value: 0 },
      { label: '1–2 servings', value: 1 },
      { label: '3+ servings', value: 2 },
    ],
  },
  {
    text: 'Do you manage your time effectively to balance study and rest?',
    options: [
      { label: 'Never', value: 0 },
      { label: 'Sometimes', value: 1 },
      { label: 'Yes, most of the time', value: 2 },
    ],
  },
  {
    text: 'How often do you engage in social activities or hobbies?',
    options: [
      { label: 'Rarely/Never', value: 0 },
      { label: 'Sometimes', value: 1 },
      { label: 'Regularly', value: 2 },
    ],
  },
  {
    text: 'Do you seek help when feeling overwhelmed or mentally stressed?',
    options: [
      { label: 'Never', value: 0 },
      { label: 'Sometimes', value: 1 },
      { label: 'Yes, I reach out for help', value: 2 },
    ],
  },
])

const answers = ref<number[]>([])
const resultMessage = ref<string>('')

function submitQuiz() {
  const score = answers.value.reduce((sum, val) => sum + (val ?? 0), 0)
  resultMessage.value =
    score <= 10
      ? '🔴 Your current lifestyle may be harming your health. Try cooking more meals, sleeping better, exercising, and seeking help when needed.'
      : score <= 16
        ? '🟡 You’re doing okay! But you can improve with better diet planning, time management, and regular physical activity.'
        : '🟢 Excellent! You have great habits that support your mental and physical health. Keep it up!'
}
</script>

<style scoped>
.quiz-section {
  background: #f5f6ef;
  color: #3a4a4a;
  padding: 2rem 1.5rem;
  border-radius: 0 0 12px 12px;
}

.habit-title {
  text-align: center;
  font-size: 2rem;
  margin-bottom: 0.5rem;
}

.intro {
  text-align: center;
  max-width: 700px;
  margin: 0 auto 1.5rem;
}

.questions-container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  margin-bottom: 1.5rem;
}

.submit-btn {
  background: #ffd700;
  color: #3a4a4a;
  padding: 0.6rem 1.2rem;
  font-size: 1rem;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  display: block;
  margin: 0 auto 1rem;
}

.submit-btn:hover {
  background: #e6c200;
}

.result-box {
  text-align: center;
  background: #e0ede7;
  color: #3a4a4a;
  padding: 1rem;
  border-radius: 8px;
  max-width: 500px;
  margin: 0 auto;
}
</style>

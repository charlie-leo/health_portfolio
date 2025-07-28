<template>
  <div>
    <h1 class="habit-title">Are Your Habits Helping or Hurting?</h1>
    <div>
      <QuestionCard
        v-for="(q, index) in questions"
        :key="index"
        :question="q"
        v-model="answers[index]"
      />
    </div>
    <button @click="submitQuiz">Submit Quiz</button>

    <div v-if="resultMessage" class="result-box">
      <h2>Result</h2>
      <p>{{ resultMessage }}</p>
    </div>

  </div>
</template>

<style scoped>
.habit-title{
  color: #3a4a4a;
}
.result-box{
  color: #3a4a4a;
}
</style>

<script setup lang="ts">
import { ref } from 'vue'
import QuestionCard from './QuestionCard.vue'

const questions = ref([
  {
    text: 'How many home-cooked meals do you eat/week?',
    options: [
      { label: '0–1', value: 0 },
      { label: '2–4', value: 1 },
      { label: '5–7', value: 2 },
    ],
  },
  {
    text: 'Do you often skip meals due to stress?',
    options: [
      { label: 'Yes', value: 0 },
      { label: 'No', value: 2 },
    ],
  },
  {
    text: 'Do you exercise 3+ times per week?',
    options: [
      { label: 'Never', value: 0 },
      { label: '1–2 times', value: 1 },
      { label: '3+ times', value: 2 },
    ],
  },
  {
    text: 'How often do you feel overwhelmed?',
    options: [
      { label: 'Often', value: 0 },
      { label: 'Sometimes', value: 1 },
      { label: 'Rarely', value: 2 },
    ],
  },
  {
    text: 'Do you use substances to cope with stress?',
    options: [
      { label: 'Yes', value: 0 },
      { label: 'Sometimes', value: 1 },
      { label: 'No', value: 2 },
    ],
  },
])

const answers = ref<number[]>([])
const resultMessage = ref<string>('')

function submitQuiz() {
  const score = answers.value.reduce((sum, val) => sum + (val ?? 0), 0)
  resultMessage.value =
    score <= 5
      ? '🔴 Your habits may be hurting you. Consider some changes.'
      : score <= 10
        ? '🟡 You’re doing okay! But there’s room to improve.'
        : '🟢 Great! Your habits are helping your health!'
}
</script>

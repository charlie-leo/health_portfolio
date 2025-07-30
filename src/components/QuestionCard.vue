<template>
  <div class="question-card">
    <h3 style="font-weight: bold">{{ question.text }}</h3>
    <div class="options-row">
      <div v-for="(opt, i) in question.options" :key="i" class="option-item">
        <input
          type="radio"
          :name="question.text"
          :value="opt.value"
          :checked="modelValue === opt.value"
          @change="$emit('update:modelValue', opt.value)"
        />
        <label>{{ opt.label }}</label>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps(['question', 'modelValue'])
defineEmits(['update:modelValue'])
</script>

<style scoped>
.question-card {
  margin-bottom: 1rem;
}

.options-row {
  display: flex;
  flex-wrap: wrap; /* Allows wrapping on small screens */
  gap: 1rem;
  margin-top: 0.5rem;
}

.option-item {
  display: flex;
  align-items: center;
  gap: 0.3rem;
}
</style>

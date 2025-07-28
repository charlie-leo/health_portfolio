<template>
    <div style="color: #3a4a4a">
      <h3>{{ question.text }}</h3>
      <div v-for="(opt, i) in question.options" :key="i" >
        <input
          type="radio"
          :name="question.text"
          :value="opt.value"
          :checked = "modelValue === opt.value"
          @change="$emit('update:modelValue', opt.value)"
        />
        <label>{{ opt.label }}</label>
      </div>
    </div>
  </template>



  <script setup lang="ts">

  defineProps(['question', 'modelValue'])
  defineEmits(['update:modelValue'])
  </script>

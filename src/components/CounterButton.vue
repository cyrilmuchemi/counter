<script setup>
import { defineEmits } from 'vue'

const emit = defineEmits(['increment'])

const handleClick = () => {
  emit('increment')
}
</script>

<template>
  <button @click="handleClick" class="counter-button"></button>
</template>

<style scoped>
.counter-button {
  padding: 10px 20px;
  font-size: 18px;
  background-color: #3498db;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.counter-button:hover {
  background-color: #2980b9;
}
</style>

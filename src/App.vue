<script setup>
import CounterButton from './components/CounterButton.vue'
import { ref } from 'vue'

const count = ref(0)

const increaseCount = () => {
  count.value += 1
}
</script>

<template>
  <h1>Vue Counter App</h1>
  <p>
    Total Clicks: <strong>{{ count }}</strong>
  </p>
  <CounterButton @increment="increaseCount" />
</template>

<style scoped></style>

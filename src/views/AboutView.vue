<script lang="ts" setup>
import { useCounterStore } from '@/stores/counter'

const counter = useCounterStore()
</script>

<template>
  <div>
    <div class="about">
      <div>
        <h1>This is an about page</h1>
      </div>
      <p>Count: {{ counter.count }}</p>
      <p>Double Count: {{ counter.doubleCount }}</p>
    </div>
    <div>
      <button @click="counter.increment()">increment</button>
      <button @click="counter.decrement()">decrement</button>
    </div>
  </div>
</template>

<style></style>

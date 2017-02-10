<template>
  <div>
    <h1>{{ counter }}</h1>
    <button @click='increment'>+</button>
    <button @click='decrement'>-</button>
    <button @click='reset'>0</button>
  </div>
</template>

<script>
import './Counter';

export default {
  name: 'counter',
  data() {
    return {
      counter: 0
    }
  },
  methods: {
    increment() {
      this.counter++;
    },
    decrement() {
      this.counter--;
    },
    reset() {
      this.counter = 0;
    }
  }
}
</script>

<style scoped>
</style>

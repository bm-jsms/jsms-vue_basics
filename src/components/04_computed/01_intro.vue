<script setup>
import { ref, computed } from 'vue';
const number = ref(5);
const square = computed(() => number.value * number.value);
const increment = () => number.value++;
</script>
<template>
	<h1>Original Number: {{ number }}</h1>
	<h1>Square: {{ square }}</h1>
	<button @click="increment">Increment</button>
</template>
<style scoped></style>

<script setup>
import { ref } from 'vue';
import ComponentEvent from './ComponentEvent.vue';

let count = ref(0);
</script>
<template>
	<h1>Count: {{ count }}</h1>
	<ComponentEvent @increment="count++" />
</template>
<style scoped></style>

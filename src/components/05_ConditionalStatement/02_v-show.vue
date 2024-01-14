<script setup>
import { ref } from 'vue';

let isVisible = ref(true);
</script>
<template>
	<p v-show="isVisible">This will show if isVisible is true</p>
	<button @click="isVisible = !isVisible">Toggle</button>
</template>
<style scoped></style>

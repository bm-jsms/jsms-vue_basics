<script setup>
import { inject } from 'vue';
const studentName = inject('studentName');
const studentAge = inject('studentAge');
const studentLocation = inject('studentLocation');
</script>
<template>
	<div>
		<h1>Student</h1>
		<p>Name: {{ studentName }}</p>
		<p>Age: {{ studentAge }}</p>
		<p>Location: {{ studentLocation }}</p>
	</div>
</template>
<style scoped></style>

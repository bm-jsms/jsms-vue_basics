<script setup>
import { provide } from 'vue';
import SchoolComponent from './School.vue';

provide('studentName', 'John Doe');
provide('studentAge', 20);
provide('studentLocation', 'London');
</script>
<template>
	<SchoolComponent />
</template>
<style scoped></style>

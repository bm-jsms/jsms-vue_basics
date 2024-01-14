<script setup>
import { ref } from 'vue';

let peoples = ref(['JSMS', 'Jhon', 'Jane']);
</script>
<template>
	<ul>
		<li v-for="person in peoples" :key="person">{{ person }}</li>
	</ul>
</template>
<style scoped></style>

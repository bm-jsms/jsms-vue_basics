<script setup>
import { ref } from 'vue';

let isUserLoggedIn = ref(true);
let uresname = 'JSMS';
let showDetails = ref(isUserLoggedIn);
</script>
<template>
	<div>
		<h1 v-if="isUserLoggedIn">Welcome {{ username }}</h1>
		<P v-else> Please login </P>
		<div v-show="showDetails">
			<h2>Details about the user</h2>
		</div>
	</div>
</template>
<style scoped></style>

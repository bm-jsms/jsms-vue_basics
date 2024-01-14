<script setup>
import { ref } from 'vue';
const formData = ref({
	username: '',
	email: '',
	password: '',
});
</script>
<template>
	<form>
		<input type="text" placeholder="username" v-model="formData.username" />
		<input type="email" placeholder="email" v-model="formData.email" />
		<input type="password" placeholder="password" v-model="formData.password" />
	</form>
	<ul>
		<li>username: {{ formData.username }}</li>
		<li>email: {{ formData.email }}</li>
		<li>password: {{ formData.password }}</li>
	</ul>
</template>
<style scoped></style>

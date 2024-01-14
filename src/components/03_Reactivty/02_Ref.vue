<script setup>
import { ref } from 'vue';

let count = ref(0);

let username = ref('');

let usersList = ref(['JSMS', 'John', 'Jordan']);
</script>

<template>
	<h1>Count: {{ count }}</h1>
	<button @click="count++">+</button>
	<button @click="count--">+</button>

	<hr />

	<h1>Username: {{ username }}</h1>
	<button @click="username = 'Alex'">Add User</button>

	<hr />

	<h1>Users List: {{ usersList }}</h1>
	<button @click="usersList.push('Matias')">Add User</button>
</template>

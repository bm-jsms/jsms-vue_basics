<script setup>
import { reactive } from 'vue';

let initialState = reactive({
	Val: {
		count: 0,
	},
	user: ['JSMS', 'Jhon'],
});
const changeUser = () => {
	initialState.user[0] = 'Jhon';
	initialState.user[1] = 'Alex';
};
</script>
<template>
	<h1>Count: {{ initialState.count }}</h1>
	<button @click="initialState.count--">Decrement</button>
	<button @click="initialState.count++">Increment</button>

	<hr />

	<h1>Users: {{ initialState.user }}</h1>
	<button @click="changeUser">Change User</button>
</template>

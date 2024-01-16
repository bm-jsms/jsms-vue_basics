<script setup>
import axios from 'axios';
import { Ref } from 'vue';
const data = ref(null);

const fetchData = async () => {
	try {
		const res = await axios.get('https://jsonplaceholder.typicode.com/posts');
		data.value = res.data;
	} catch (error) {
		console.error(error);
	}
};
</script>
<template>
	<div>
		<h1>Using Axios</h1>
		<button @click="fetchData">Fetch Data</button>
		<div>
			<h2>Axios Data</h2>
			<pre>{{ data }} </pre>
		</div>
	</div>
</template>
<style scoped></style>

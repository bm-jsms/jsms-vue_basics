<script setup>
import { ref } from 'vue';
const data = ref(null);

const fetchData = () => {
	fetch('https://jsonplaceholder.typicode.com/posts')
		.then(response => {
			if (!response.ok) {
				throw new Error('Network response was not ok');
			}
			return response.json();
		})
		.then(jsonResponse => {
			data.value = jsonResponse;
		})
		.catch(error => {
			console.error(
				'There has been a problem with your fetch operation:',
				error,
			);
		});
};
</script>
<template>
	<div>
		<h1>Using Fetch API</h1>
		<button @click="fetchData">Fetch Data</button>
		<div>
			<h2>FetchData</h2>
			<pre>{{ data }} </pre>
		</div>
	</div>
</template>
<style scoped></style>

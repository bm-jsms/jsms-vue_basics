<script setup>
import { defineAsyncComponent, ref } from 'vue';

const showComponent = ref(false);
const renderComponent = defineAsyncComponent(() => import('./Component.vue'));
</script>
<template>
	<div>
		<h1>Async Component</h1>
		<p>Click the button to load the component</p>
		<div v-if="showComponent">
			<renderComponent />
		</div>
		<button @click="showComponent = !showComponent">show | hide</button>
	</div>
</template>
<style scoped></style>

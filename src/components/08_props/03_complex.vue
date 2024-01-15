<script setup>
defineProps({
	frieds: {
		type: Array,
		required: true,
	},
	userInfo: {
		type: Object,
		required: true,
	},
});
</script>
<template>
	<ul v-for="friend in frieds" :key="friend">
		<li>{{ friend }}</li>
	</ul>
</template>
<style scoped></style>

<script setup>
const isTrue = true;
const isFalse = false;
</script>
<template>
	<div>
		<p v-if="isTrue">This will show if isTrue is true</p>
		<p v-else-if="isFalse">This will show if isFalse is true</p>
		<p v-else>This will show if both are false</p>
	</div>
</template>
<style scoped></style>

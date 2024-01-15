<script setup>
import { ref } from 'vue';
import SPComponent from './01_SPComponent.vue';
import dynamic from './02_dynamic.vue';
import Complex from './03_complex.vue';

const firstName = ref('JSMS');
const lastName = ref('BM');
</script>
<template>
	<SPComponent name="JSMS" />

	<hr />

	<dynamic :firstName="firstName" :lastName="lastName" />

	<hr />

	<Complex
		:frieds="['jsms', 'john', 'jane']"
		:userInfo="{ firstName: 'Daniel', age: 20 }"
	/>
</template>
<style scoped></style>

<script setup>
const myTitle = 'Text Interpolation';

const myFn = message => {
	return message;
};

const myNumber = 10;
</script>

<template>
	<h1>
		{{ myTitle }}
	</h1>
	<p>
		{{ myFn('This is a function') }}
	</p>
	<p>My number is: {{ myNumber }}</p>
</template>

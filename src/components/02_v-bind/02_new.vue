<script setup>
const myLink = 'https://github.com';
const imageLink =
	'https://images.unsplash.com/photo-1561037404-61cd46aa615b?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D';
const imageAlt = 'a beautiful puppy';
const imageWidth = 300;
const imageHeight = 200;
</script>

<template>
	<h2>Go to GitHub: <a :href="myLink">GitHub</a></h2>
	<hr />
	<h2>
		{{ imageAlt }}
	</h2>
	<img
		:src="imageLink"
		:alt="imageAlt"
		:width="imageWidth"
		:height="imageHeight"
	/>
</template>

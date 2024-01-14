<script setup>
const myImage = {
	link: 'https://images.unsplash.com/photo-1561037404-61cd46aa615b?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D',
	alt: 'a beautiful puppy',
	width: 300,
	height: 200,
};
</script>

<template>
	<img :="myImage" />
</template>

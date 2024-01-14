import { ref } from 'vue';
<script setup>
import { ref } from 'vue';

let books = ref([
	{
		id: 1,
		title: 'The Way of Kings',
		autor: 'Brandon Sanderson',
		genre: 'Fantasy',
		year: 2010,
	},
	{
		id: 2,
		title: 'The Name of the Wind',
		autor: 'Patrick Rothfuss',
		genre: 'Fantasy',
		year: 2007,
	},
	{
		id: 3,
		title: 'The Final Empire',
		autor: 'Brandon Sanderson',
		genre: 'Fantasy',
		year: 2006,
	},
	{
		id: 4,
		title: 'The Well of Ascension',
		autor: 'Brandon Sanderson',
		genre: 'Fantasy',
		year: 2007,
	},
	{
		id: 5,
		title: 'The Hero of Ages',
		autor: 'Brandon Sanderson',
		genre: 'Fantasy',
		year: 2008,
	},
	{
		id: 6,
		title: 'The Alloy of Law',
		autor: 'Brandon Sanderson',
		genre: 'Fantasy',
		year: 2011,
	},
	{
		id: 7,
		title: 'The Way of Kings',
		autor: 'Brandon Sanderson',
		genre: 'Fantasy',
		year: 2010,
	},
	{
		id: 8,
		title: 'The Name of the Wind',
		autor: 'Patrick Rothfuss',
		genre: 'Fantasy',
		year: 2007,
	},
	{
		id: 9,
		title: 'The Final Empire',
		autor: 'Brandon Sanderson',
		genre: 'Fantasy',
		year: 2006,
	},
	{
		id: 10,
		title: 'The Well of Ascension',
		autor: 'Brandon Sanderson',
		genre: 'Fantasy',
		year: 2007,
	},
]);
</script>
<template>
	<h1>Books</h1>

	<ul v-for="{ id, title, autor, genre, year } in books" :key="id">
		<li>Title: {{ title }}</li>
		<li>Autor: {{ autor }}</li>
		<li>Genre: {{ genre }}</li>
		<li>Year: {{ year }}</li>
	</ul>
</template>
<style scoped></style>

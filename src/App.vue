<script setup>
// imports
// import HelloWorld from '@/components/00_intro/HelloWorld.vue';
import SlotComponent from '@/components/10_slots/01_intro.vue';
import NamedSlotComponent from '@/components/10_slots/02_NamedSlot.vue';
</script>

<template>
	<div>
		<SlotComponent>
			<h1>My Title</h1>
			<p>My Content</p>
		</SlotComponent>
	</div>
	<div>
		<NamedSlotComponent>
			<template #title>
				<h1>My Title</h1>
			</template>
			<template #content>
				<p>My Content</p>
			</template>
		</NamedSlotComponent>

		<NamedSlotComponent>
			<template #content>
				<p>My Content</p>
			</template>
			<template #title>
				<h1>My Title</h1>
			</template>
		</NamedSlotComponent>
	</div>
</template>

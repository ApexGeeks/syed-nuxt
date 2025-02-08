<script setup lang="ts">
import { Vue3Marquee } from 'vue3-marquee';

const _ltrAdjectives = [
	'Dynamic',
	'Customized',
	'Efficient',
	'Versatile',
	'Creative',
	'Innovative',
	'Good',
	'Dynamic',
	'Customized',
	'Efficient',
	'Versatile',
	'Creative',
	'Innovative',
	'Good'
];
</script>

<template>
	<div class="mt-10">
		<Vue3Marquee
			:duration="15"
			clone
			direction="reverse"
		>
			<div
				class="flex flex-nowrap overflow-hidden *:px-2 *:pt-2 *:pb-3 *:text-6xl *:leading-[1.1] *:font-semibold"
			>
				<h1
					class="border-l-4 border-teal-400 bg-gradient-to-r from-teal-200 to-teal-100"
				>
					Innovative
				</h1>
				<h1
					class="border-l-4 border-blue-400 bg-gradient-to-r from-blue-200 to-blue-100"
				>
					Creative
				</h1>
				<h1
					class="border-l-4 border-purple-400 bg-gradient-to-r from-purple-200 to-purple-100"
				>
					Dynamic
				</h1>
				<h1
					class="border-l-4 border-teal-400 bg-gradient-to-r from-teal-200 to-teal-100"
				>
					Customized
				</h1>
				<h1
					class="border-l-4 border-blue-400 bg-gradient-to-r from-blue-200 to-blue-100"
				>
					Efficient
				</h1>
				<h1
					class="border-l-4 border-purple-400 bg-gradient-to-r from-purple-200 to-purple-100"
				>
					Versatile
				</h1>
			</div>
		</Vue3Marquee>
		<div class="py-3" />
		<Vue3Marquee
			:duration="15"
			clone
		>
			<div
				class="flex flex-nowrap overflow-hidden *:px-2 *:pt-2 *:pb-3 *:text-6xl *:leading-[1.1] *:font-semibold"
			>
				<h1
					class="border-l-4 border-teal-400 bg-gradient-to-r from-teal-200 to-teal-100"
				>
					Expert
				</h1>
				<h1
					class="border-l-4 border-purple-400 bg-gradient-to-r from-purple-200 to-purple-100"
				>
					Next-Gen
				</h1>
				<h1
					class="border-l-4 border-blue-400 bg-gradient-to-r from-blue-200 to-blue-100"
				>
					Responsive
				</h1>
				<h1
					class="border-l-4 border-teal-400 bg-gradient-to-r from-teal-200 to-teal-100"
				>
					Strategic
				</h1>
				<h1
					class="border-l-4 border-purple-400 bg-gradient-to-r from-purple-200 to-purple-100"
				>
					Collaborative
				</h1>
				<h1
					class="border-l-4 border-blue-400 bg-gradient-to-r from-blue-200 to-blue-100"
				>
					Progressive
				</h1>
			</div>
		</Vue3Marquee>
	</div>
</template>

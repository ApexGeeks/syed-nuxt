<script setup lang="ts">
const runtimeConfig = useRuntimeConfig();
</script>

<template>
	<div
		class="font-Poppins text-Black container flex flex-col items-center py-20"
	>
		<img
			src="/images/heading.png"
			alt=""
			class="max-w-64 cursor-pointer transition-all hover:scale-110"
		/>
		<h3 class="my-5 mt-16 text-lg font-semibold">
			Helping Businesses Transition to AI
		</h3>
		<div class="flex flex-col items-center">
			<h1
				class="font-Poppins max-w-sm text-center text-4xl leading-snug font-bold md:text-7xl"
			>
				Next-Gen
			</h1>
			<span
				class="border-Green from-GreenLight font-Poppins max-w-xl border-l-4 bg-gradient-to-r to-transparent pl-2 text-center text-5xl leading-snug font-bold md:text-7xl"
			>
				AI Voice Agents
			</span>
		</div>
		<div
			class="mt-5 gap-3 *:my-3 *:block max-sm:w-full max-sm:*:mx-auto max-sm:*:w-full max-sm:**:w-full sm:flex"
		>
			<a
				:href="runtimeConfig.public.calendly"
				target="_blank"
			>
				<Button
					class="inline-flex items-center justify-center gap-2 shadow-lg shadow-gray-300 max-sm:w-full"
				>
					<Icon
						name="mynaui:telephone"
						size="20"
					/>
					Book A Call</Button
				>
			</a>
			<a href="#pricing">
				<Button
					is-light
					class="max-sm:mt-3 max-sm:w-full max-sm:text-start"
					>View Selection</Button
				>
			</a>
		</div>
	</div>
</template>

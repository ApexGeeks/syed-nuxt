<script setup lang="ts">
const runtimeConfig = useRuntimeConfig();
</script>

<template>
	<div
		class="font-Poppins text-Black container flex flex-col items-center pt-20 pb-40 md:pb-28"
	>
		<img
			src="/images/heading.png"
			alt=""
			class="max-w-64 cursor-pointer transition-all hover:scale-110"
		/>
		<h3 class="my-5 mt-24 text-lg font-semibold">
			Helping Businesses Transition to AI
		</h3>
		<div class="flex flex-col items-center">
			<h1
				class="font-Poppins max-w-sm text-center text-4xl leading-snug font-bold md:text-7xl"
			>
				Advanced
			</h1>
			<span
				class="border-Green from-GreenLight font-Poppins max-w-2xl border-l-4 bg-gradient-to-r to-transparent pl-2 text-center text-5xl leading-snug font-bold md:text-7xl"
			>
				AI Text Chatbots
			</span>
		</div>
		<div class="mt-5 gap-3 *:my-3 max-sm:*:mx-auto max-sm:*:w-full sm:flex">
			<a
				:href="runtimeConfig.public.calendly"
				target="_blank"
			>
				<Button
					class="inline-flex items-center justify-center gap-2 shadow-lg shadow-gray-300 max-sm:w-full"
					><img
						src="https://cdn.prod.website-files.com/66b3f7d1ff69e1e7133402fc/66b3f7d1ff69e1e713340363_Phone.svg"
						alt=""
					/>Book A Call</Button
				>
			</a>
			<a href="#pricing">
				<Button
					is-light
					class="max-sm:mt-3 max-sm:w-full max-sm:text-start"
					>Discover Pricing</Button
				>
			</a>
		</div>
	</div>
</template>

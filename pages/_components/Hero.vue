<script setup lang="ts">
const runtimeConfig = useRuntimeConfig();

const isMounted = ref(false);

onMounted(() => {
	setTimeout(() => {
		isMounted.value = true;
	}, 500);
});
</script>

<template>
	<div
		class="font-Poppins text-Black container flex flex-col items-center py-20 transition duration-300"
		:class="isMounted ? 'translate-y-0 opacity-100' : 'translate-y-5 opacity-0'"
	>
		<img
			src="/images/heading.png"
			alt=""
			class="max-w-64 cursor-pointer transition-all hover:scale-110"
		/>
		<h3 class="my-5 mt-16 text-lg font-semibold">
			Helping Businesses Transition to AI
		</h3>
		<h1
			class="font-Poppins max-w-2xl text-center text-7xl leading-snug font-bold"
		>
			Building
			<span
				class="border-Green from-GreenLight border-l-4 bg-gradient-to-r to-transparent pl-2"
			>
				AI Agents
			</span>
			that do real work.
		</h1>
		<div
			class="mt-5 gap-3 *:my-3 *:block max-sm:w-full max-sm:*:mx-auto max-sm:*:w-full max-sm:**:w-full sm:flex"
		>
			<a
				:href="runtimeConfig.public.calendly"
				target="_blank"
			>
				<Button class="flex items-center gap-2">
					<Icon
						name="mynaui:telephone"
						size="20"
					/>
					Book A Call
				</Button>
			</a>
			<a href="#services">
				<Button
					is-light
					class="max-sm:text-start"
					>Our Services</Button
				>
			</a>
			<a href="#ai-agents">
				<Button
					is-light
					class="max-sm:text-start"
					>What are AI Agents?</Button
				>
			</a>
		</div>
	</div>
</template>

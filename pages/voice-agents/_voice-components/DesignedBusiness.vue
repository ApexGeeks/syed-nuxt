<script setup lang="ts">
const runtimeConfig = useRuntimeConfig();
</script>

<template>
	<div class="py-5 md:py-32">
		<div
			id="pricing"
			class="container mt-20"
		>
			<h1
				class="mb-14 w-50 text-xl font-semibold max-sm:mx-auto md:mb-24 md:w-full md:text-5xl"
			>
				Designed for any
				<span
					class="border-l-4 border-teal-400 bg-gradient-to-r from-teal-200 to-teal-100"
					>Business</span
				>
			</h1>
			<div
				id="pricing"
				class="mt-5 rounded-[32px] border border-gray-100 bg-[#fbfbfb] p-3"
			>
				<div class="rounded-[20px] border border-gray-100 bg-white p-6">
					<h1
						class="mb-7 text-3xl font-semibold max-sm:max-w-64 max-sm:text-2xl"
					>
						Inbound Phone Agent
					</h1>
					<p class="font-medium">
						Inbound AI Phone Agents are virtual systems that use artificial
						intelligence, including natural language processing and speech
						recognition, to handle incoming customer calls. They can interpret
						caller queries, provide relevant responses, and resolve issues
						without the need for human agents. These systems help businesses
						improve efficiency, reduce operational costs, and offer 24/7
						customer support.
					</p>
				</div>
			</div>
			<div
				id="pricing"
				class="mt-5 rounded-[32px] border border-gray-100 bg-[#fbfbfb] p-3"
			>
				<div class="rounded-[20px] border border-gray-100 bg-white p-6">
					<h1
						class="mb-7 text-3xl font-semibold max-sm:max-w-64 max-sm:text-2xl"
					>
						Outbound Phone Agent
					</h1>
					<p class="font-medium">
						Outbound AI Phone Agents are AI-driven systems that autonomously
						initiate phone calls to customers for tasks like appointment
						reminders. They use natural language processing and speech synthesis
						to engage in conversations, answer questions, and record responses.
						These agents help businesses maintain consistent communication with
						customers.
					</p>
				</div>
			</div>
			<div
				class="container mt-6 flex flex-col items-center justify-between gap-5 rounded-4xl bg-white px-6 py-6 md:mt-10 md:flex-row md:px-10 md:py-10"
			>
				<h1 class="text-xl font-semibold md:text-2xl">
					Book Our AI Agent Discovery Call Today.
				</h1>
				<a
					target="_blank"
					:href="runtimeConfig.public.calendly"
					class="cursor-pointer"
				>
					<div
						class="bg-Black flex items-center gap-2 rounded-full px-20 py-4 text-white"
					>
						<img
							src="https://cdn.prod.website-files.com/66b3f7d1ff69e1e7133402fc/66b3f7d1ff69e1e713340363_Phone.svg"
							alt=""
						/>Book A Call
					</div>
				</a>
			</div>
		</div>
	</div>
</template>

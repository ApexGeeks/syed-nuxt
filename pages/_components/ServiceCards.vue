<script setup lang="ts">
import ServicesImage from './ServicesImage.vue';
</script>

<template>
	<div
		class="container mt-10 rounded-4xl border border-gray-100 bg-white pb-10"
	>
		<div
			class="flex flex-col items-start justify-between px-10 py-8 md:flex-row md:items-center"
		>
			<h1 class="mb-4 text-3xl font-semibold md:mb-0 md:text-4xl">
				Our Services
			</h1>
			<p
				class="rounded-full bg-[#10d07f1a] px-4 py-1.5 font-semibold text-[#0a955a]"
			>
				3 services
			</p>
		</div>
		<div class="grid gap-5 *:min-h-90">
			<ServicesImage
				image="/images/phone-girl.jpg"
				class="col-start-1 -col-end-1"
			>
				<template #heading>AI Voice Agents</template>
				<template #paragraph>
					Next Level AI Voice Agents For Automated Inbound and Outbound Phone
					Calls
				</template>
			</ServicesImage>
			<ServicesImage
				image="/images/phone-girl.jpg"
				class="col-start-2 col-end-3"
			>
				<template #heading>AI Voice Agents</template>
				<template #paragraph>
					Next Level AI Voice Agents For Automated Inbound and Outbound Phone
					Calls
				</template>
			</ServicesImage>
			<ServicesImage
				image="/images/phone-girl.jpg"
				class="col-start-1 col-end-3"
			>
				<template #heading>AI Voice Agents</template>
				<template #paragraph>
					Next Level AI Voice Agents For Automated Inbound and Outbound Phone
					Calls
				</template>
			</ServicesImage>
		</div>
		<div
			class="mx-10 mt-5 mb-10 rounded-[32px] border border-gray-100 bg-[#fbfbfb] p-3"
		>
			<div class="rounded-[20px] border border-gray-100 bg-white p-6">
				<h1 class="mb-7 text-3xl font-semibold">What Are AI Agents?</h1>
				<p class="text-[17px] font-semibold">
					AI agents are like digital employees, capable of handling tasks
					autonomously to drive business growth. Examples include AI phone
					agents that can handle call inquiries, website chatbots for customer
					support, and email agents for sales and support. These agents interact
					with stakeholders, providing efficient and scalable solutions to
					enhance business operations.
				</p>
			</div>
		</div>
		<div
			class="mx-10 mt-5 rounded-[32px] border border-gray-100 bg-[#fbfbfb] p-3"
		>
			<div class="rounded-[20px] border border-gray-100 bg-white p-6">
				<h1 class="mb-7 text-3xl font-semibold">
					Unsure how AI could be used in your business?
				</h1>
				<p class="mb-6 text-[17px] font-semibold">
					If you're unsure how AI could benefit your business, feel free to book
					a 30-minute or 1-hour consultation session with Brendan Jowett. During
					the session, you'll learn how we've successfully implemented AI in
					businesses similar to yours, providing insights to help you make a
					more informed decision.
				</p>
				<button
					class="rounded-full bg-black px-7 py-4 font-semibold text-white transition-all duration-200 hover:pr-10 hover:pl-10"
				>
					Book 1:1 Consultation Session
				</button>
			</div>
		</div>
	</div>
</template>

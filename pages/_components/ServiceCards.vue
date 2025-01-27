<script setup>
import image1 from '@/assets/images/phone-girl.jpg';
import image2 from '@/assets/images/laptop-boy.jpg';
import image3 from '@/assets/images/headphone.webp';
</script>

<template>
	<div
		class="mx-auto mt-10 max-w-[80%] rounded-4xl border border-gray-100 bg-white pb-10"
	>
		<div class="flex items-center justify-between px-10 py-8">
			<h1 class="text-4xl font-semibold">Our Services</h1>
			<p
				class="rounded-full bg-[#10d07f1a] px-4 py-1.5 font-semibold text-[#0a955a]"
			>
				3 services
			</p>
		</div>
		<div class="flex flex-col items-center">
			<div
				class="grid grid-cols-1 grid-rows-[400px] gap-4 px-10 md:grid-cols-2"
			>
				<div class="relative h-auto overflow-hidden rounded-2xl">
					<img
						:src="image1"
						alt=""
						class="absolute z-[5] rounded-2xl transition-all hover:scale-105"
					/>
					<div class="relative z-[10] flex items-end justify-start p-5">
						<h1 class="mb-3 text-2xl font-semibold text-white">
							AI Voice Agents
						</h1>
						<p class="mb-3 text-xl font-semibold text-[#fbfbfb99] opacity-60">
							Next level AI Voice Agents For Automated Inbound & Outbound Phone
							Calls.
						</p>
						<button class="text-xl font-semibold text-white">
							Get Started
						</button>
					</div>
				</div>
				<div class="relative overflow-hidden">
					<img
						:src="image2"
						alt=""
						class="absolute z-[5] rounded-2xl transition-all hover:scale-105"
					/>
					<div class="relative z-[10] flex items-end justify-start p-5">
						<h1 class="mb-3 text-2xl font-semibold text-white">
							AI Voice Agents
						</h1>
						<p
							class="mb-3 w-[60%] text-xl font-semibold text-[#fbfbfb99] opacity-60"
						>
							Next level AI Voice Agents For Automated Inbound & Outbound Phone
							Calls.
						</p>
						<button class="text-xl font-semibold text-white">
							Get Started
						</button>
					</div>
				</div>
			</div>
			<div class="relative mb-5 px-10">
				<img
					:src="image3"
					alt=""
					class="rounded-2xl transition-all"
				/>
				<div class="absolute bottom-10 left-8">
					<h1 class="mb-3 text-2xl font-semibold text-white">
						AI Voice Agents
					</h1>
					<p
						class="mb-3 w-[60%] text-xl font-semibold text-[#fbfbfb99] opacity-60"
					>
						Next level AI Voice Agents For Automated Inbound & Outbound Phone
						Calls.
					</p>
					<button class="text-xl font-semibold text-white">Get Started</button>
				</div>
			</div>
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

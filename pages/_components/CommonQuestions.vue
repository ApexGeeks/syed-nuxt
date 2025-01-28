<script setup>
import { Collapse } from 'vue-collapsed';
const isExpanded = ref(false);
</script>

<template>
	<div class="container mx-auto px-5">
		<h1 class="mb-14 ml-16 text-2xl font-medium">Common Questions</h1>
		<div class="grid grid-cols-1 gap-4 md:grid-cols-2">
			<div class="flex flex-col gap-4">
				<div
					class="mb-3 cursor-pointer gap-y-5 rounded-[24px] bg-white px-[24px] py-[32px] font-semibold"
				>
					<div
						class="flex w-full items-start justify-between"
						@click="isExpanded = !isExpanded"
					>
						<button class="text-start">
							What types of AI Agents do you offer?
						</button>
						<div class="relative">
							<button class="h-[2px] w-[17px] bg-black" />
							<button
								class="absolute right-[7px] bottom-[-1px] h-[17px] w-[2px] bg-black transition-transform duration-300 ease-in-out"
								:class="{ 'rotate-90': isExpanded }"
							/>
						</div>
					</div>
					<Collapse :when="isExpanded">
						<p
							class="text-[18px]"
							:class="{ 'mt-5': isExpanded }"
						>
							We provide two types of AI Agents. AI Voice Agents & AI Text
							Chatbots.
						</p>
					</Collapse>
				</div>
				<div
					class="mb-3 cursor-pointer gap-y-5 rounded-[24px] bg-white px-[24px] py-[32px] font-semibold"
				>
					<div
						class="flex w-full items-start justify-between"
						@click="isExpanded = !isExpanded"
					>
						<button class="text-start">
							How do you ensure the quality of your projects?
						</button>
						<div class="relative">
							<button class="h-[2px] w-[17px] bg-black" />
							<button
								class="absolute right-[7px] bottom-[-1px] h-[17px] w-[2px] bg-black transition-transform duration-300 ease-in-out"
								:class="{ 'rotate-90': isExpanded }"
							/>
						</div>
					</div>
					<Collapse :when="isExpanded">
						<p
							class="text-[18px]"
							:class="{ 'mt-5': isExpanded }"
						>
							We have a minimum 2 week testing period for our AI Agents. Our
							packages range from 2 weeks of testing to 6 weeks of testing. If
							you opt for our maintenance package, you will receive immediate
							upgrades & bug fixes.
						</p>
					</Collapse>
				</div>
				<div
					class="mb-3 cursor-pointer gap-y-5 rounded-[24px] bg-white px-[24px] py-[32px] font-semibold"
				>
					<div
						class="flex w-full items-start justify-between"
						@click="isExpanded = !isExpanded"
					>
						<button class="text-start">
							What is your development process like?
						</button>
						<div class="relative">
							<button class="h-[2px] w-[17px] bg-black" />
							<button
								class="absolute right-[7px] bottom-[-1px] h-[17px] w-[2px] bg-black transition-transform duration-300 ease-in-out"
								:class="{ 'rotate-90': isExpanded }"
							/>
						</div>
					</div>
					<Collapse :when="isExpanded">
						<p
							class="text-[18px]"
							:class="{ 'mt-5': isExpanded }"
						>
							Our process involves initial consultation, planning, design,
							development, testing, and deployment. We follow agile
							methodologies to ensure flexibility and responsiveness.
						</p>
					</Collapse>
				</div>
			</div>
			<div class="flex flex-col gap-4">
				<div
					class="mb-3 cursor-pointer gap-y-5 rounded-[24px] bg-white px-[24px] py-[32px] font-semibold"
				>
					<div
						class="flex w-full items-start justify-between"
						@click="isExpanded = !isExpanded"
					>
						<button class="text-start">
							How do you handle project timelines?
						</button>
						<div class="relative">
							<button class="h-[2px] w-[17px] bg-black" />
							<button
								class="absolute right-[7px] bottom-[-1px] h-[17px] w-[2px] bg-black transition-transform duration-300 ease-in-out"
								:class="{ 'rotate-90': isExpanded }"
							/>
						</div>
					</div>
					<Collapse :when="isExpanded">
						<p
							class="text-[18px]"
							:class="{ 'mt-5': isExpanded }"
						>
							We create detailed project timelines with clear milestones. Our
							project deadlines are met by coordinating all phases of the
							development process.
						</p>
					</Collapse>
				</div>
				<div
					class="mb-3 cursor-pointer gap-y-5 rounded-[24px] bg-white px-[24px] py-[32px] font-semibold"
				>
					<div
						class="flex w-full items-start justify-between"
						@click="isExpanded = !isExpanded"
					>
						<button class="text-start">
							How often will I receive updates on the project?
						</button>
						<div class="relative">
							<button class="h-[2px] w-[17px] bg-black" />
							<button
								class="absolute right-[7px] bottom-[-1px] h-[17px] w-[2px] bg-black transition-transform duration-300 ease-in-out"
								:class="{ 'rotate-90': isExpanded }"
							/>
						</div>
					</div>
					<Collapse :when="isExpanded">
						<p
							class="text-[18px]"
							:class="{ 'mt-5': isExpanded }"
						>
							We will have at least 1 call per week to discuss the status of the
							project during its development & testing phase.
						</p>
					</Collapse>
				</div>
			</div>
		</div>
	</div>
</template>

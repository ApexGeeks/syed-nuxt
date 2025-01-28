<script setup>
import { Collapse } from 'vue-collapsed';
const questions = reactive([
	{
		title: 'What types of AI Agents do you offer?',
		answer:
			'We provide two types of AI Agents. AI Voice Agents & AI Text Chatbots.',
		isExpanded: false
	},
	{
		title: 'How do you ensure the quality of your projects?',
		answer:
			'We have a minimum 2-week testing period for our AI Agents. Our packages range from 2 weeks to 6 weeks of testing, with maintenance for upgrades & fixes.',
		isExpanded: false
	},
	{
		title: 'What is your development process like?',
		answer:
			'Our process involves initial consultation, planning, design, development, testing, and deployment.',
		isExpanded: false
	},
	{
		title: 'How do you handle project timelines?',
		answer:
			'We create detailed project timelines with clear milestones and ensure deadlines are met.',
		isExpanded: false
	},
	{
		title: 'How often will I receive updates on the project?',
		answer:
			'We schedule at least 1 call per week during the development and testing phases.',
		isExpanded: false
	}
]);
const expandHandler = (question) => {
	return (question.isExpanded = !question.isExpanded);
};
</script>

<template>
	<div class="container mx-auto px-5">
		<h1 class="mb-14 ml-16 text-2xl font-medium">Common Questions</h1>
		<div class="grid grid-cols-1 gap-4 md:grid-cols-2">
			<div class="flex flex-col gap-1">
				<div
					v-for="question in questions.slice(0, 3)"
					:key="question.title"
					class="mb-3 cursor-pointer gap-y-5 rounded-[24px] bg-white px-[24px] py-[32px] font-semibold"
				>
					<div
						class="flex w-full items-start justify-between"
						@click="expandHandler(question)"
					>
						<button class="text-start">
							{{ question.title }}
						</button>
						<div class="relative cursor-pointer">
							<button class="h-[2px] w-[17px] bg-black" />
							<button
								class="absolute right-[7px] bottom-[-1px] h-[17px] w-[2px] bg-black transition-transform duration-300 ease-in-out"
								:class="{ 'rotate-90': question.isExpanded }"
							/>
						</div>
					</div>
					<Collapse :when="question.isExpanded">
						<p
							class="text-[18px]"
							:class="{ 'mt-5': question.isExpanded }"
						>
							{{ question.answer }}
						</p>
					</Collapse>
				</div>
			</div>
			<div class="flex flex-col gap-1">
				<div
					v-for="question in questions.slice(3)"
					:key="question.title"
					class="mb-3 cursor-pointer gap-y-5 rounded-[24px] bg-white px-[24px] py-[32px] font-semibold"
				>
					<div
						class="flex w-full items-start justify-between"
						@click="expandHandler(question)"
					>
						<button class="text-start">
							{{ question.title }}
						</button>
						<div class="relative cursor-pointer">
							<button class="h-[2px] w-[17px] bg-black" />
							<button
								class="absolute right-[7px] bottom-[-1px] h-[17px] w-[2px] bg-black transition-transform duration-300 ease-in-out"
								:class="{ 'rotate-90': question.isExpanded }"
							/>
						</div>
					</div>
					<Collapse :when="question.isExpanded">
						<p
							class="text-[18px]"
							:class="{ 'mt-5': question.isExpanded }"
						>
							{{ question.answer }}
						</p>
					</Collapse>
				</div>
			</div>
		</div>
	</div>
</template>

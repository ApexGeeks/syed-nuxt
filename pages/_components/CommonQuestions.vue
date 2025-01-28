<script setup lang="ts">
import Question from './Question.vue';
</script>

<template>
	<section class="font-Poppins bg-[#f4f4f4] py-20">
		<div class="container">
			<h1 class="text-4xl font-semibold">Common Questions</h1>
			<div class="mt-10 grid gap-5 md:grid-cols-2">
				<div class="flex flex-col gap-5 *:w-full">
					<Question>
						<template #heading>What types of AI Agents do you offer?</template>
						<template #text>
							We provide two types of AI Agents. AI Voice Agents & AI Text
							Chatbots.
						</template>
					</Question>
					<Question>
						<template #heading>What types of AI Agents do you offer?</template>
						<template #text>
							We provide two types of AI Agents. AI Voice Agents & AI Text
							Chatbots.
						</template>
					</Question>
					<Question>
						<template #heading>What types of AI Agents do you offer?</template>
						<template #text>
							We provide two types of AI Agents. AI Voice Agents & AI Text
							Chatbots.
						</template>
					</Question>
				</div>
				<div class="flex flex-col gap-5 *:w-full">
					<Question>
						<template #heading>What types of AI Agents do you offer?</template>
						<template #text>
							We provide two types of AI Agents. AI Voice Agents & AI Text
							Chatbots.
						</template>
					</Question>
					<Question>
						<template #heading>What types of AI Agents do you offer?</template>
						<template #text>
							We provide two types of AI Agents. AI Voice Agents & AI Text
							Chatbots.
						</template>
					</Question>
					<Question>
						<template #heading>What types of AI Agents do you offer?</template>
						<template #text>
							We provide two types of AI Agents. AI Voice Agents & AI Text
							Chatbots.
						</template>
					</Question>
				</div>
			</div>
		</div>
	</section>
</template>

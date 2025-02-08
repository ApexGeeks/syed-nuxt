<script setup lang="ts">
import ChatbotAdjective from './_chatbots-components/ChatbotAdjective.vue';
import ChatbotConnect from './_chatbots-components/ChatbotConnect.vue';
import ChatbotContact from './_chatbots-components/ChatbotContact.vue';
import ChatbotHero from './_chatbots-components/ChatbotHero.vue';
import ChatbotPricing from './_chatbots-components/ChatbotPricing.vue';
import ChatbotQuestion from './_chatbots-components/ChatbotQuestion.vue';
const isFooterInView = ref(false);
</script>
<template>
	<!-- eslint-disable vue/no-multiple-template-root -->

	<div class="bg-gray-100">
		<Navbar :show-navbar="isFooterInView" />
		<ChatbotHero />
		<ChatbotAdjective />
	</div>
	<div class="bg-gray-100">
		<ChatbotPricing />
		<ChatbotQuestion />
		<ChatbotConnect />
		<ChatbotContact />
	</div>
	<Footer @is-in-view="(value: boolean) => (isFooterInView = !value)" />
</template>

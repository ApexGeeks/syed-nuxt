<script setup lang="ts">
import SupportAdjectives from './_support-components/SupportAdjectives.vue';
import SupportConnect from './_support-components/SupportConnect.vue';
import SupportContact from './_support-components/SupportContact.vue';
import SupportHero from './_support-components/SupportHero.vue';
import SupportPricing from './_support-components/SupportPricing.vue';
import SupportQuestions from './_support-components/SupportQuestions.vue';

const isFooterInView = ref(false);
</script>

<template>
	<!-- eslint-disable vue/no-multiple-template-root -->
	<Navbar :show-navbar="isFooterInView" />
	<div class="bg-gray-100">
		<SupportHero />
		<SupportAdjectives />
	</div>
	<div class="bg-gray-200">
		<SupportPricing />
	</div>
	<div class="bg-gray-100">
		<SupportQuestions />
		<SupportConnect />
		<SupportContact />
	</div>

	<Footer @is-in-view="(value: boolean) => (isFooterInView = !value)" />
</template>

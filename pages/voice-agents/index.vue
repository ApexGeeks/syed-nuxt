<script lang="ts" setup>
import AgentAdjectives from './_voice-components/AgentAdjectives.vue';
import AgentConnect from './_voice-components/AgentConnect.vue';
import AgentContact from './_voice-components/AgentContact.vue';
import AgentHero from './_voice-components/AgentHero.vue';
import AgentPricing from './_voice-components/AgentPricing.vue';
import DesignedBusiness from './_voice-components/DesignedBusiness.vue';
const isFooterInView = ref(false);
</script>

<template>
	<!-- eslint-disable vue/no-multiple-template-root -->
	<div class="bg-gray-100">
		<Navbar :show-navbar="isFooterInView" />
		<AgentHero />
		<AgentAdjectives />
	</div>
	<div class="bg-gray-200 pb-40 md:px-24">
		<DesignedBusiness />
		<AgentPricing />
		<AgentConnect />
		<AgentContact />
	</div>
	<Footer @is-in-view="(value: boolean) => (isFooterInView = !value)" />
</template>

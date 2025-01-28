<script setup>
import Hero from './_components/Hero.vue';
import Adjectives from './_components/Adjectives.vue';
import Benifits from './_components/Benifits.vue';
import CommonQuestions from './_components/CommonQuestions.vue';
import OurServices from './_components/OurServices.vue';
import ServiceCards from './_components/ServiceCards.vue';
import Connect from './_components/Connect.vue';
import Contact from './_components/Contact.vue';
</script>

<template>
	<!-- eslint-disable vue/no-multiple-template-root -->
	<Navbar />
	<Hero />
	<Adjectives />
	<ServiceCards />
	<Benifits />
	<OurServices />
	<CommonQuestions />
	<Connect />
	<Contact />
	<Footer />
</template>

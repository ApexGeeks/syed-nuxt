<script setup lang="ts">
const runtimeConfig = useRuntimeConfig();
</script>

<template>
	<section
		id="contact-us"
		class="bg-[#f4f4f4] py-20"
		data-aos="fade-up"
		data-aos-offset="400"
		data-aos-duration="1000"
	>
		<div class="container">
			<div class="flex items-center justify-between gap-5 max-sm:flex-col">
				<h1 class="text-4xl font-semibold">
					Let's
					<span
						class="border-l-4 border-blue-400 bg-gradient-to-tr from-blue-200 to-blue-50 pr-5 pl-1"
					>
						Connect
					</span>
				</h1>
				<p class="max-w-60 font-medium max-sm:text-center">
					We're here to answer your questions and discuss how we can help you
					achieve your goals.
				</p>
			</div>
			<div class="mt-10 rounded-3xl bg-white p-10 sm:mx-5">
				<CalendlyInlineWidget :url="runtimeConfig.public.calendly" />
			</div>
		</div>
	</section>
</template>

<script setup lang="ts">
const runtimeConfig = useRuntimeConfig();
</script>

<template>
	<section class="mt-64 pt-20 pb-14">
		<div class="container">
			<div
				class="flex items-start justify-start gap-5 max-sm:flex-col md:items-center md:justify-between"
			>
				<h1 class="text-xl font-semibold max-sm:mb-5 max-sm:ml-16 md:text-4xl">
					Let's
					<span
						class="border-l-4 border-blue-400 bg-gradient-to-tr from-blue-200 to-blue-50 pr-5 pl-1"
					>
						Connect
					</span>
				</h1>
				<p
					class="max-w-70 text-start text-[15px] font-medium max-sm:pl-10 md:max-w-72"
				>
					We're here to answer your questions and discuss how we can help you
					achieve your goals.
				</p>
			</div>
			<div class="mt-16 rounded-3xl bg-[#fbfbfb] py-6 max-sm:pl-6">
				<CalendlyInlineWidget :url="runtimeConfig.public.calendly" />
			</div>
		</div>
	</section>
</template>

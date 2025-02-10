<script setup lang="ts">
const footerRef = ref();
const emits = defineEmits<{ (id: 'isInView', value: boolean): void }>();

const isFooterVisible = useElementVisibility(footerRef, {
	rootMargin: '-100px'
});

watch(
	isFooterVisible,
	(isVisisble) => {
		emits('isInView', isVisisble);
	},
	{
		immediate: true
	}
);
</script>

<template>
	<footer
		ref="footerRef"
		class="bg-Black py-10"
	>
		<div
			class="container flex flex-col justify-between gap-16 max-md:items-center md:flex-row"
		>
			<img
				src="/images/heading-white.png"
				alt=""
				class="mt-10 w-50 md:self-start"
			/>
			<div class="max-w-[350px]">
				<div class="grid grid-cols-2 md:grid-cols-[100px_200px]">
					<div>
						<p class="mt-3 text-sm text-[#9b9a99]">Menu</p>
					</div>
					<div>
						<ul
							class="space-y-3 text-xl text-white *:cursor-pointer *:transition *:duration-300 *:hover:opacity-80"
						>
							<li>
								<a href="#services"> Services </a>
							</li>
							<li><a href="#pricing">Pricing</a></li>
							<li><a href="#contact-us">Contact Us</a></li>
							<li>1:1 Consultation</li>
							<li class="text-red-500">Youtube Channel</li>
						</ul>
					</div>
				</div>
				<p class="mt-10 text-sm text-[#9b9a99] max-md:text-center">
					© INFLATE AI 2023 - 2025, All rights reserved. Ground floor, 470 St
					Kilda Road, Melbourne VIC 3004
				</p>
			</div>
		</div>
	</footer>
</template>

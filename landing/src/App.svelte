<script>
	import Hero from "./components/Hero.svelte";
	import Product from "./components/Product.svelte";
	import Faq from "./components/Faq.svelte";
	import Conversion from "./components/Conversion.svelte";
	import Logo from "./components/Logo.svelte";
	let y = 0;
	const heightOfHero = 100;
</script>

<svelte:window bind:scrollY={y} />

<main
	class="relative bg-gradient-to-tr from-primary-200 to-white min-h-screen text-slate text-sm sm:text-base flex flex-col"
>
	<div class="inset-0 opacity-10 absolute z-[997] bgGrid"></div>
	<div class="z-[998]">
		{#if y >= 100}
			<div class="fixed left-0 top-3 z-[999]" style="width: 100%;">
				<div
					class="border-1 max-w-[1400px] mx-auto w-full flex items-center justify-between p-4 py-6 dropShadow rounded-full pr-8 fadeIn bar"
				>
					<a href="#" class="flex gap-2 text-primary-700">
						<Logo />
						<h1 class="font-semibold">Venome</h1>
					</a>
					<nav class="hidden md:flex items-center gap-4 lg:gap-6">
						<a
							href="#project"
							class="duration-200 hover:text-primary-700 cursor-pointer"
							>Project Overview</a
						>
						<a
							href="#who-made-venome"
							class="duration-200 hover:text-primary-700 cursor-pointer"
							>Who made Venome?</a
						>
					</nav>
				</div>
			</div>
		{/if}
		<Hero />
		<Product />
		<Faq />
		<Conversion />
	</div>
</main>

<style>
	.bar {
		background-color: rgba(255, 255, 255, 0.75);
		backdrop-filter: blur(10px);
		-webkit-backdrop-filter: blur(10px);
		border: 2px solid white;
	}
</style>

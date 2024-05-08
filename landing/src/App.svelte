<script>
	import Hero from "./components/Hero.svelte";
	import Product from "./components/Product.svelte";
	import Review from "./components/Review.svelte";
	import Faq from "./components/Faq.svelte";
	import Conversion from "./components/Conversion.svelte";
</script>

<main
	class="relative bg-gradient-to-tr from-slate-800 to-slate-900 min-h-screen text-white text-sm sm:text-base flex flex-col"
>
	<div class="inset-0 opacity-10 absolute z-[998] bgGrid"></div>
	<div class="z-[999]">
		<Hero />
		<Product />
		<Review />
		<Faq />
		<Conversion />
	</div>
</main>

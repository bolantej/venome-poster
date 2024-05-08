<script>
	import SectionWrap from "./SectionWrap.svelte";
	import Header from "./Header.svelte";
	import Cta from "./Cta.svelte";
	import Star from "./Star.svelte";
</script>

<SectionWrap>
	<Header />
	<div
		class="flex flex-col gap-10 flex-1 items-center justify-center pb-10 md:pb-14"
	>
		<h2
			class="text-5xl sm:text-6xl md:text-7xl lg:text-8xl max-w-[1200px] mx-auto w-full text-center font-semibold"
		>
			<span class="font-extralight text-">The Unknown</span>
			<span class="text-primary-700">Venome</span>
		</h2>
		<p
			class="text-xl sm:text-2xl md:text-3xl max-w-[1000px] mx-auto w-full font-light"
		>
			<i>Accelerating</i> venom protein research with a platform to
			<span class="font-medium">Store</span>,
			<span class="font-medium">Visualize</span>, and
			<span class="font-medium">Analyze</span>
			venom proteins with computation.
		</p>
		<Cta />
	</div>
</SectionWrap>

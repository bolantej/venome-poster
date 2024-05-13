<script>
	import SectionWrap from "./SectionWrap.svelte";
	import Header from "./Header.svelte";
	import Cta from "./Cta.svelte";
	import NewTabLink from "./NewTabLink.svelte";
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
			A website to
			<span class="font-medium">Store</span> and
			<span class="font-medium">Analyze</span> hundreds of
			<span class="font-medium">Venom Proteins</span>
			from the
			<NewTabLink href="https://venombiochemistrylab.weebly.com/"
				>Venom Biochemistry & Molecular Biology Lab</NewTabLink
			>
			at Oregon State University
		</p>
		<Cta />
	</div>
</SectionWrap>

<script>
	import ProductCard from "./ProductCard.svelte";
	import SectionWrap from "./SectionWrap.svelte";
</script>

<SectionWrap id="project">
	<div
		class="flex flex-col gap-10 sm:gap-14 md:gap-24 flex-1 items-center justify-center pb-10 md:-bottom-1/4"
	>
		<div class="flex flex-col gap-2">
			<p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
				A collections of genes is a genome. A collection of venoms is a <span
					class="font-bold">venome</span
				>.
			</p>
			<h3
				class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-extralight text-center"
			>
				Explore <span class="font-medium">The Venome</span>
			</h3>
		</div>

		<ProductCard videoSrc="search-demo.mov">
			<slot>
				<span class="text-primary-700">Search</span> Hundreds of Venom Proteins
			</slot>
			<slot slot="description">
				<p class="font-light">
					<span class="font-medium"
						>Find the protein you're looking for.</span
					> You can keyword search the Venom Lab's over 400 proteins found
					in wasp venoms. You can narrow down the possibilities by applying
					length, weight, or organism filters too.
				</p>
			</slot>
		</ProductCard>

		<ProductCard reverse videoSrc="view-demo.mov">
			<slot>
				<span class="text-primary-700">View</span> protein structure
			</slot>
			<slot slot="description">
				<p class="font-light">
					<span class="font-medium"
						>Interact with the protein directly.</span
					>
					You can view the 3D structure of the protein and learn about
					the provided information (like organism, method, and more). You
					can also view computed algorithms on the data in the
					<i>Computed Insights</i> section of the protein.
				</p>
			</slot>
		</ProductCard>

		<ProductCard>
			<slot>
				<span class="text-primary-700">Compare</span> similar proteins
			</slot>
			<slot slot="description">here yee</slot>
		</ProductCard>

		<ProductCard reverse>
			<slot>
				<span class="text-primary-700">Learn</span> with interactive articles
			</slot>
			<slot slot="description">here yee</slot>
		</ProductCard>
	</div>
</SectionWrap>

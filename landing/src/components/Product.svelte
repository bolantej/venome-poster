<script>
	import ProductCard from "./ProductCard.svelte";
	import SectionWrap from "./SectionWrap.svelte";
	import NewTabLink from "./NewTabLink.svelte";
</script>

<SectionWrap id="project">
	<div style="height: 100px; display: hidden;"></div>
	<div
		class="flex flex-col gap-10 sm:gap-14 md:gap-24 flex-1 items-center justify-center pb-10 md:-bottom-1/4"
		id="project"
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


		<ProductCard reverse videoSrc="view-demo.mov">
			<slot>
				<span class="text-primary-700">Compare</span> between protein prediction softwares
			</slot>
			<slot slot="description">
				<p class="font-light">
					<span class="font-medium"
						>Find the differences between AlphaFold 2 and AlphaFold 3.</span
					>
					Swap between between the different predictions for each protein to find the similarities
					and differences.

				</p>
			</slot>
		</ProductCard>

		<ProductCard videoSrc="align-demo.mov">
			<slot>
				<span class="text-primary-700">Manage</span> protein uploads and users
			</slot>
			<slot slot="description">
				<p class="font-light">
					<span class="font-medium"
						>Improved site moderation and protein approval system.</span
					>
					Admins of the site now have the ability to approve and deny protein uploads requested by the users.
					There is also now a user interface for the admins to manage the users directly in the site, including
					the ability to delete users, and promote them to admins, as well as look through their uploaded proteins.
				</p>
			</slot>
		</ProductCard>

		<ProductCard videoSrc="search-demo.mov">
			<slot>
				<span class="text-primary-700">Sort</span> your searches
			</slot>
			<slot slot="description">
				<p class="font-light">
					<span class="font-medium"
						>Look through the smallest and largest proteins.</span
					> You can sort by any of the computed insighted that we have 
					  calculated on the site as well as filtering by them too.
				</p>
			</slot>
		</ProductCard>

		<ProductCard reverse videoSrc="article-demo.mov">
			<slot>
				<span class="text-primary-700">View</span> new computed insights
			</slot>
			<slot slot="description">
				<p class="font-light">
					<span class="font-medium"
						>Look through the most relevant proteins in PDB database and the atom count for each protein.</span
					>
					Use <NewTabLink
					href="https://github.com/steineggerlab/foldseek"
					icon>Foldseek</NewTabLink
					> to find other proteins from the <NewTabLink
					href="https://www.rcsb.org/"
					icon>PDB Databank</NewTabLink
					> that are structually similar to proteins in our venome database. Additionally the atom count is
					now displayed for each protein.
				</p>
			</slot>
		</ProductCard>
	</div>
</SectionWrap>

<script>
	import { Video, VideoPlaceholder } from "flowbite-svelte";
	export let reverse = false;
</script>

<div
	class="grid grid-cols-1 md:grid-cols-2 gap-14 md:gap-16 lg:gap-20 relative text-base"
>
	<div
		class={"flex flex-col gap-8 md:gap-10 pt-10 " +
			(reverse ? " md:order-2" : " ")}
	>
		<h4
			class="text-2xl sm:text-3xl md:text-4xl max-w-[1000px] w-full font-medium pr-10 relative after:absolute after:top-full after:left-0 after:w-1/5 after:h-1.5 after:mt-1 after:bg-primary-950"
		>
			<slot />
		</h4>
		<p><slot name="description" /></p>
	</div>
	<div class={"flex flex-col dropShadow overflow-hidden rounded-b-lg "}>
		<div
			class="rounded-t-xl h-5 sm:h-8 bg-white opacity-60 flex items-center gap-1 pl-2"
		>
			{#each [1, 2, 3] as i}
				<div
					class="rounded-full aspect-square w-2.5 sm:w-3 bg-primary-300 ml-1"
				></div>
			{/each}
		</div>
		<div class="flex flex-col flex-1">
			<!-- <img src={""} alt="product-img" /> -->
			<Video src="test.mov" autoplay controls loop />
		</div>
	</div>
</div>

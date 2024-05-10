<script>
	import { Button } from "flowbite-svelte";
	import {
		GithubSolid,
		ArrowRightOutline,
		FilePdfSolid,
		ArrowDownOutline,
	} from "flowbite-svelte-icons";
	export let reverse = false;
</script>

<div class="flex items-center gap-4 justify-center flex-wrap">
	<Button size="lg" color="primary" pill href="#project"
		>Project Overview <span
			style={reverse ? "transform: rotate(180deg);" : ""}
			><ArrowDownOutline class="ml-1" /></span
		>
	</Button>
	<Button
		size="lg"
		color="light"
		pill
		href="https://github.com/xnought/venome"
		>Open Source <GithubSolid class="ml-1" size="lg" />
	</Button>
	<Button
		size="lg"
		color="light"
		pill
		href="https://github.com/Venom-Biochem-Lab/venome-poster/blob/main/posters/2024.TheUnknownVenome.CS.094.pdf"
		>2024 Engineering Expo Poster <FilePdfSolid class="ml-1" />
	</Button>
	<Button size="lg" color="primary" disabled pill
		>Live Website (🚧 Coming Soon) <ArrowRightOutline
			class="ml-1"
		/></Button
	>
</div>

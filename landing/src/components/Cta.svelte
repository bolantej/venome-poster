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
	<Button size="lg" color="dark" pill href="#project"
		>Project Overview <span
			style={reverse ? "transform: rotate(180deg);" : ""}
			><ArrowDownOutline class="ml-1" /></span
		>
	</Button>
	<Button
		size="lg"
		color="light"
		pill
		href="https://github.com/venom-biochem-lab/venome"
		target="_blank"
		>Open Source <GithubSolid class="ml-1" size="lg" />
	</Button>
	<Button
		size="lg"
		color="light"
		pill
		href="https://github.com/bolantej/venome-poster/blob/main/posters/2025.ExpoPoster.034.pdf"
		target="_blank"
		>2025 Engineering Expo Poster <FilePdfSolid class="ml-1" />	
	</Button>
	<Button
		size="lg"
		color="light"
		pill
		href="https://venom-biochem-lab.github.io/venome-poster/#project"
		target="_blank"
		>2024 Capstone Landing Page <FilePdfSolid class="ml-1" />
	</Button>
	<Button
		size="lg"
		color="primary"
		pill
		href="https://venome.cqls.oregonstate.edu"
		>Live Website<ArrowRightOutline class="ml-1" /></Button
	>
</div>

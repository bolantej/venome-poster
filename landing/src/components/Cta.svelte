<script>
	import { Button } from "flowbite-svelte";
	import {
		GithubSolid,
		ArrowRightOutline,
		FilePdfSolid,
	} from "flowbite-svelte-icons";
</script>

<div class="flex items-center gap-4">
	<Button size="lg" color="light" href="https://github.com/xnought/venome"
		>Open Source <GithubSolid class="ml-1" size="lg" />
	</Button>
	<Button
		size="lg"
		color="light"
		href="https://github.com/Venom-Biochem-Lab/venome-poster/blob/main/posters/2024.TheUnknownVenome.CS.094.pdf"
		>2024 Engineering Expo Poster <FilePdfSolid class="ml-1" />
	</Button>
	<Button size="lg" color="primary" disabled
		>Get Started (🚧 Coming Soon) <ArrowRightOutline class="ml-1" /></Button
	>
</div>

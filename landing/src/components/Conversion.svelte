<script>
	import { PlusOutline } from "flowbite-svelte-icons";
	import Cta from "./Cta.svelte";
</script>

<section
	class="py-14 md:py-20 flex flex-col gap-8 bg-slate-800 text-white text-center items-center justify-center"
>
	<h4 class="text-xl sm:text-2xl md:text-3xl poppins">
		Quick <span class="poppins font-bold">Links</span>
	</h4>
	<p class="poppins text-base sm:text-lg md:text-xl flex gap-2 items-center">
		<span class="x"><PlusOutline /></span> Store and Analyze Venom Proteins
		<span class="x"><PlusOutline /></span>
	</p>
	<Cta reverse />
</section>

<style>
	.x {
		animation: turn 2s infinite ease-in-out;
	}
	@keyframes turn {
		from {
			transform: rotate(0deg);
		}
		to {
			transform: rotate(360deg);
		}
	}
</style>

<script>
	import { ArrowUpRightFromSquareOutline } from "flowbite-svelte-icons";

	export let href = "";
	export let icon = false;
	export let iconSize = "sm";
</script>

<a
	{href}
	target="_blank"
	class="underline duration-200 hover:text-primary-700 cursor-pointer"
>
	<slot />{#if icon}<ArrowUpRightFromSquareOutline
			size={iconSize}
			class="inline"
		/>{/if}
</a>

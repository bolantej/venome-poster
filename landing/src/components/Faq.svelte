<script>
	import { Button } from "flowbite-svelte";
	import { ArrowUpRightFromSquareOutline } from "flowbite-svelte-icons";
	import SectionWrap from "./SectionWrap.svelte";
	let people = [
		{
			name: "Ethan Peterson",
			link: "https://github.com/EthanPeterson55?tab=repositories",
			description:
				"Senior undergrad, School of EECS at Oregon State University",
		},
		{
			name: "Jace Bolante",
			link: "https://github.com/bolantej",
			description:
				"Senior undergrad, School of EECS at Oregon State University.",
		},
		{
			name: "Megan Dorn",
			link: "https://github.com/MDorn03",
			description:
				"Senior undergrad, School of EECS at Oregon State University.",
		},
		{
			name: "Alex Clark",
			link: "https://github.com/arc25275",
			description:
				"Senior undergrad, School of EECS at Oregon State University.",
		},
		{
			name: "Alex Holly",
			link: "https://github.com/AlexHolly007",
			description:
				"Senior undergrad, School of EECS at Oregon State University",
		},
		{
			name: "Chase Copeland",
			link: "https://github.com/chasec22",
			description:
				"Senior undergrad, School of EECS at Oregon State University",
		},
		{
			name: "Michael Youkhateh",
			link: "https://biochem.oregonstate.edu/directory/michael-youkhateh",
			description:
				"PhD Student, Department of Biochemistry & Biophysics, Venom Biochemistry Lab.",
		},
		{
			name: "Dr. Nathan Mortimer",
			link: "https://biochem.oregonstate.edu/directory/nathan-mortimer",
			description:
				"Associate Professor, Department of Biochemistry & Biophysics, Linus Pauling Institute, Venom Biochemistry Lab.",
		},
		{
			name: "2024 Venome Capstone Group",
			link: "https://venom-biochem-lab.github.io/venome-poster/",
			description:
				"Donald (Donny) Bertucci, Ansen Garvin, Cora Bailey, and Amanda Sinha",
		},
	];
</script>

<SectionWrap id="who-made-venome">
	<div
		class="flex flex-col gap-10 sm:gap-14 md:gap-24 py-20 flex-1 items-center justify-center"
	>
		<div class="flex flex-col gap-2">
			<p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
				Who made Venome?
			</p>
			<h3
				class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-regular text-center"
			>
				<span>Brought to you by</span>
			</h3>
		</div>

		<div class="flex flex-col gap-4 sm:gap-5 md:gap-7 w-full">
			{#each people as p}
				<div
					class="flex flex-col gap-2 text-left max-w-[800px] w-full mx-auto relative p-4 px-6"
				>
					<div
						class="absolute top-0 left-0 w-1/3 h-[1px] bg-slate-950 -translate-x-4"
					></div>
					<div
						class="absolute top-0 left-0 h-2/3 w-[1px] bg-slate-950 -translate-y-4"
					></div>
					<h4
						class="text-lg sm:text-xl md:text-2xl pt-2 flex items-center gap-2"
					>
						{p.name}
						{#if "link" in p}
							<Button
								size="xs"
								pill
								outline
								href={p.link}
								target="_blank"
							>
								Personal Site <ArrowUpRightFromSquareOutline
									class="ml-1"
									size="sm"
								/>
							</Button>
						{/if}
					</h4>
					<p class="p-2">{p.description}</p>
				</div>
			{/each}
		</div>
	</div>
</SectionWrap>

<script>
	import { Button } from '#lib/components/ui/button/index.ts';

	const items = [
		{
			title: 'pieisspy.github.io',
			summary: 'My portfolio website (you are right here!)',
			repository: 'https://github.com/PieIsSpy/pieisspy.github.io'
		},
		{
			title: 'pieisspy.neocities.org',
			summary: 'My personal website, mostly containing blogs',
			repository: 'https://github.com/PieIsSpy/pieisspy.neocities.org'
		},
		{
			title: 'Plants-Vs-Zombies',
			summary: 'A recreation of Plants Vs Zombies written in Java',
			repository: 'https://github.com/PieIsSpy/Plants-Vs-Zombies'
		},
		{
			title: 'Pokemon-Gen-1-Save-Reader',
			summary: 'A Pokemon Gen 1 Save File Reader written in C',
			repository: 'https://github.com/PieIsSpy/Pokemon-Gen-1-Save-Reader'
		},
		{
			title: 'SokobanGB',
			summary: 'A recreation of Sokoban in Game Boy using C and GBDK',
			repository: 'https://github.com/PieIsSpy/SokobanGB'
		},
		{
			title: 'odin-etch-a-sketch',
			summary: 'A simple website for drawing using Javascript DOM manipulation',
			repository: 'https://github.com/PieIsSpy/odin-etch-a-sketch'
		}
	];
</script>

<main class="mx-auto flex w-full max-w-2xl flex-col gap-6 px-4 py-12">
	<h2 class="text-2xl font-bold tracking-tight">Repositories</h2>

	<div class="grid grid-cols-1 gap-4 sm:grid-cols-2">
		{#each items as item}
			<div class="flex flex-col justify-between gap-4 rounded-lg border bg-card p-6 text-card-foreground shadow-sm">
				<div class="flex flex-col gap-2">
					<h3 class="text-lg font-semibold tracking-tight">{item.title}</h3>
					<p class="text-sm text-muted-foreground">{item.summary}</p>
				</div>

				{#if item.repository}
					<div>
						<Button
							href={item.repository}
							target="_blank"
							rel="noreferrer"
							size="sm"
							class="rounded-sm"
						>
							Repository
						</Button>
					</div>
				{/if}
			</div>
		{/each}
	</div>
</main>
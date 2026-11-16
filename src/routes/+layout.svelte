<script lang="ts">
	import './layout.css';
	import favicon from '#lib/assets/favicon.svg';
	import type { LayoutProps } from './$types';
	import { resolve } from '$app/paths';

	let { children }: LayoutProps = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<header>
	<nav class="flex justify-between items-center rounded-lg border bg-muted p-6 text-card-foreground shadow-sm">
		<a href={resolve('/')}>PieIsSpy</a>

		<div class="flex gap-2">
			<a href={resolve('/')}>Home</a>
			<a href={resolve('/repositories')}>Repositories</a>
			<a href={resolve('/animations')}>Animations</a>
		</div>
	</nav>
</header>

{@render children()}

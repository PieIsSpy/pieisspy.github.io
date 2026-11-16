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
	<nav class="flex justify-between items-center">
		<a href={resolve('/')}>Site Name</a>

		<div>
			<a href={resolve('/')}>Home</a>
			<a href={resolve('/repositories')}>Repositories</a>
			<a href={resolve('/animations')}>Animations</a>
		</div>
	</nav>
</header>

{@render children()}

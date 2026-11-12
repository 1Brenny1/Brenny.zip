<script lang="ts">
	import './layout.css';
	import favicon from '#lib/assets/favicon.svg';
	import type { LayoutProps } from './$types';
	import Header from '#lib/components/Header/Header.svelte';
	import Footer from '#lib/components/Footer/Footer.svelte';

	let { children }: LayoutProps = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>Brenny.zip</title>
</svelte:head>

<div class="h-screen grid grid-rows-[auto_1fr_auto]">
	<Header />

	<main class="p-4 space-y-4 w-full max-w-5xl mx-auto">
		{@render children()}
	</main>

	<Footer />
</div>
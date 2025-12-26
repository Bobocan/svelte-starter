<script lang="ts">
	import "./layout.css";
	import favicon from "$lib/assets/favicon.svg";

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<header class="sticky top-0 flex gap-4 px-4 py-2 border-b">
	<a href="/" class="text-blue-600 hover:underline">Home</a>
	<a href="/about" class="text-blue-600 hover:underline">About</a>
</header>

{@render children()}

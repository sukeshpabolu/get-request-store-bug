<script>
	import './global.css';
	import { bundlePath } from '$lib/bundle.js';

	/** @type {{children?: import('svelte').Snippet}} */
	let { children } = $props();
</script>

<svelte:head>
	<title>Example app</title>
	<script defer={true} src={bundlePath}></script>
</svelte:head>

{@render children?.()}

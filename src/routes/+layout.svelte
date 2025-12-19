<script>
	import './layout.css';
	import favicon from '$lib/assets/favicon.ico';
	import share_image from '$lib/assets/preview-screenshot.png';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<meta name="title" property="og:title" content="The Button">
	<meta name="description" property="og:description" content="To press, or not to press?">
	<meta name="image" property="og:image" content={share_image}>
	<meta name="url" property="og:url" content="button.tighebrary.io">
</svelte:head>

{@render children()}

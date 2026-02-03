<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/ma_logo.png';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<!-- Google tag (gtag.js) -->
	<script async src="https://www.googletagmanager.com/gtag/js?id=G-ZP77ZZMX6X"></script>
	<script>
		window.dataLayer = window.dataLayer || [];
		function gtag(){dataLayer.push(arguments);}
		gtag('js', new Date());
		gtag('config', 'G-ZP77ZZMX6X');
	</script>
</svelte:head>
{@render children()}

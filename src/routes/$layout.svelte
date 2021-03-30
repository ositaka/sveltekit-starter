<script>
	import Nav from '$lib/Nav.svelte';
</script>

<header>
	<Nav />
</header>

<slot />

<style>
	:root {
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell,
			'Open Sans', 'Helvetica Neue', sans-serif;
	}

	:global(body) {
		overflow: hidden;
	}

	:global(main) {
		position: absolute;
		width: 100%;
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
</style>

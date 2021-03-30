<script>
	import Nav from '$lib/Nav.svelte';
</script>

<header>
	<Nav />
</header>

<slot />
<img src="/img/1.png" alt="" style="visibility: hidden" />
<img src="/img/2.png" alt="" style="visibility: hidden" />

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

<script>
	import Nav from '$lib/Nav.svelte';
</script>

<header>
	<Nav />
</header>

<slot></slot>

<style>
	:root {
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell,
			'Open Sans', 'Helvetica Neue', sans-serif;
	}

	:global( body ) {
		overflow: hidden;
	}
</style>
<script>
	import Nav from '$lib/Nav.svelte';
	import LocaleSwitcher from '$lib/LocaleSwitcher.svelte';
</script>

<header>
	<Nav />
	<LocaleSwitcher />
</header>

<main>
    <slot></slot>
</main>

<style>
	:root {
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell,
			'Open Sans', 'Helvetica Neue', sans-serif;
	}

	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
</style>
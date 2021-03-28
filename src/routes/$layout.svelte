<script>
	import Nav from '$lib/Nav.svelte';
	import { setupI18n, isLocaleLoaded, locale, dir } from '../services/i18n';
	import LocaleSwitcher from '$lib/LocaleSwitcher.svelte';

	$: if (!$isLocaleLoaded) {
        setupI18n({ withLocale: 'en' });
    }
    $: { document.dir = $dir; }
</script>

{#if $isLocaleLoaded}

	<header>
		<Nav />
		<LocaleSwitcher />
	</header>

	<main>
		<slot></slot>
	</main>

{:else}
    <p>Loading...</p>
{/if}

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
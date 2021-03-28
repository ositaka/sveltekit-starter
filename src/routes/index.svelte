<svelte:head>
	<title>Home</title>
	<meta name="description" content="The Home page description." />
</svelte:head>


<script>
	import { _ } from '../services/i18n';
    import LocaleSwitcher from '$lib/LocaleSwitcher.svelte';
	import Counter from '$lib/Counter.svelte';
</script>

<h1>{$_('home.topic')}</h1>
<h2>{$_('home.subtopic')}</h2>
<hr />
<h1>Hello world!</h1>

<Counter />
<LocaleSwitcher />

<style>
	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4rem;
		font-weight: 100;
		line-height: 1.1;
		margin: 4rem auto;
		max-width: 14rem;
	}

	@media (min-width: 480px) {
		h1 {
			max-width: none;
		}
	}
</style>

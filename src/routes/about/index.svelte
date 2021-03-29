<svelte:head>
	<title>About</title>
	<meta name="description" content="The about page description." />
</svelte:head>


<script>
	import Counter from '$lib/Counter.svelte';
</script>

<h1>About Page!</h1>

<!-- <h1>{$_('home.topic')}</h1>
<h2>{$_('home.subtopic')}</h2> -->
<Counter />

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

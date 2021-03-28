<svelte:head>
	<title>Team</title>
	<meta name="description" content="The Team page description." />
</svelte:head>


<script>
	import Counter from '$lib/Counter.svelte';
</script>

<h1>Team Page!</h1>

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

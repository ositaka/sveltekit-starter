<script>
	import { send, receive } from '$lib/Crossfade.js';
	import Counter from '$lib/Counter.svelte';
</script>

<svelte:head>
	<title>Team</title>
	<meta name="description" content="The Team page description." />
</svelte:head>

<main>
	<img
		style="width: 100vw; position: absolute; left: -10px; top: -50px; z-index: -1;"
		out:send={{ key: 'borat' }}
		in:receive={{ key: 'borat' }}
		alt="Borat"
		src="/img/1.png"
	/>
	<h1 out:send={{ key: 'h1' }} in:receive={{ key: 'h1' }}>Best team on earth!</h1>

	<Counter />
</main>

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

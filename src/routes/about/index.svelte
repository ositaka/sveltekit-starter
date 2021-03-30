<script>
	import { send, receive } from '$lib/Crossfade.js';
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="The about page description." />
</svelte:head>

<main>
	<img
		style="max-width: 30vw;"
		out:send={{ key: 'borat' }}
		in:receive={{ key: 'borat' }}
		alt="Borat"
		src="/img/2.png"
	/>
	<h1 out:send={{ key: 'h1' }} in:receive={{ key: 'h1' }}>About the world!</h1>
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

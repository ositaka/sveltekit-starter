<svelte:head>
	<title>Home</title>
	<meta name="description" content="The Home page description." />
</svelte:head>


<script>
	import { send, receive } from '$lib/Crossfade.js';
</script>

<main>
	<h1 out:send="{{key: 'h1'}}" in:receive="{{key: 'h1'}}">Hello world!</h1>
	<img out:send="{{key: 'borat'}}" in:receive="{{key: 'borat'}}" alt='Borat' src='https://apef.pt/wp-content/uploads/2020/05/placeholder.png'>
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

	main {
		position: absolute;
		width: 100%;
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
</style>

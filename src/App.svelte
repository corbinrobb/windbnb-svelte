<script>
	import Header from './components/Header.svelte';
import Results from './components/Results.svelte';
</script>

<main>
	<Header/>
	<Results/>
</main>

<style>
	main {
		text-align: center;
		padding: 3em;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
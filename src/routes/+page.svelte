<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/low-poly-grid-haikei.svg';
	import welcome_fallback from '$lib/images/low-poly-grid-haikei.svg';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Carbon: Gamified task management" />
</svelte:head>

<section>
	<h1>
		<span class="welcome">
			<picture>
				<source srcset={welcome} type="image/webp" />
				<img src={welcome_fallback} alt="Welcome" />
			</picture>
		</span>

		to your new<br />SvelteKit app
	</h1>

	<h2>
		try editing <strong>src/routes/+page.svelte</strong>
	</h2>

	<Counter />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}
</style>

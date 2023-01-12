<script>
	import Brand from '$lib/Brand.svelte';
	import Links from '$lib/Links.svelte';
	import Motto from '$lib/Motto.svelte';
</script>

<div class="home">
	<div id="brand">
		<Brand />
	</div>
	<div id="links">
		<Links />
	</div>

	<div id="motto">
		<Motto />
	</div>
	<article id="intro">
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla iusto tenetur cupiditate quasi
		cum. Ipsam eius perferendis aliquid tempore itaque dolorem, quibusdam sapiente sunt quaerat, vel
		adipisci ea? Eius, dignissimos.
	</article>

	<main id="main">
		<img class="umstud-home" src="/umstud-home.png" />
	</main>
</div>

<style>
	.home {
		display: grid;
		grid-template-areas:
			'brand . links'
			'motto main main'
			'intro main main';
		grid-template-rows: 6em 9em 1fr;
		grid-template-columns: 20em 1fr 14em;
		min-height: 100vh;
	}
	.home > * {
		border: 1px solid black;
		display: block;
	}
	#brand {
		grid-area: brand;
		padding: 0.5em;
		text-transform: capitalize;
	}
	#links {
		grid-area: links;
	}
	#motto {
		grid-area: motto;
	}

	#intro {
		grid-area: intro;
		padding: 1em;
		text-align: justify;
	}
	#main {
		grid-area: main;
	}
</style>

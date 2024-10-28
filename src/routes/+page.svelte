<script>
	import crest from '$lib/images/crest.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Home page description" />
</svelte:head>

<section>
	<h1>Clan-Mckinnon</h1>
	<div class="hero">
		<img style="width: 200px" src={crest} alt="Crest" />
	</div>
</section>

<style>
	section {
		justify-content: center;
		align-items: center;
	}
	
	.hero {
		text-align: center;
	}

	.hero img {
		width: 400px;
	}
</style>

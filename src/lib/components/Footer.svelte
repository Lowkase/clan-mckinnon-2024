<script>
	import { page } from '$app/stores';
</script>

<footer>
	<div class="content">FOOTER</div>
	<div class="source">lib/components/Footer.svelte. included in routes/+layout</div> 
</footer>

<style>
	div {
		text-align: center;
	}
	
	div.content {
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-align: center;
		text-transform: uppercase;
		letter-spacing: 0.1em;		
		margin-bottom: 10px;
	}

	div:last-child {
		margin-bottom: 0;
	}

	footer {
		background: #323232;
		padding: 20px;
	}
</style>

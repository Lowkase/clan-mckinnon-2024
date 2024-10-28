<script>
	import { page } from '$app/stores';
</script>

<header>
	<div>
		<nav>
			<ul>
				<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
					<a href="/">Home</a>
				</li>
				<li aria-current={$page.url.pathname === '/404' ? 'page' : undefined}>
					<a href="/404">404</a>
				</li>
			</ul>
		</nav>
	</div>
	<div class="source">lib/components/Header.svelte. included in routes/+layout</div> 
</header>

<style>
	.source {
		text-align: center;
		padding-bottom: 20px;
	}

	header {
		background: #323232;
	}

	nav {
		display: flex;
		justify-content: center;
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	li a:hover {
		color: var(--color-theme-2);
	}

	li[aria-current='page'] a{
		color: var(--color-theme-1);		
	}
</style>

<script>
	import './styles.css';
</script>

<div class="app">
	<main>
	<p>use:enhance only works well when paired with a SvelteKit action</p>
		<article>
		  <slot />
		</article>
		<p>Ideally, we'd have a more useful dev only error message when doesn't post to a SvelteKit action.</p>
		<p>Alternatively, we could handle the non-JSON responses better.</p>
	</main>
</div>

<style>
article {
	background-color: #ddd;
	padding: 1rem;
}
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>

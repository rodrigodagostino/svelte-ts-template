<script lang="ts">
	import svelteLogo from './lib/assets/images/svelte-logo.svg';
	import Counter from './lib/components/Counter.svelte';
</script>

<main class="app-main">
	<div class="container">
		<div>
			<a href="https://svelte.dev" target="_blank" rel="noreferrer">
				<img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
			</a>
		</div>
		<h1>Welcome to Svelte</h1>
		<p>Visit <a href="https://svelte.dev/">svelte.dev</a> to read the documentation.</p>
		<Counter />
	</div>
</main>
<footer class="app-footer">
	<div class="container">
		<a
			href="https://github.com/rodrigodagostino/vite-svelte-ts-template"
			target="_blank"
			rel="noreferrer"
		>
			Made with <img src={svelteLogo} alt="Svelte.js logo" /> by Rodrigo D’Agostino
		</a>
	</div>
</footer>

<style lang="scss">
	.container {
		max-width: 54rem;
		margin: 0 auto;
		padding: 1rem;
		position: relative;
	}

	.app-main {
		margin-top: 24vh;

		img {
			width: 6rem;
			height: auto;
			margin: 0 auto;
		}

		h1 {
			margin: 2rem 0 0.5rem;
		}

		p {
			margin-bottom: 2rem;
		}
	}

	.app-footer {
		font-size: 0.875rem;
		text-align: center;
		margin-top: auto;

		.container {
			display: flex;
			justify-content: center;
			padding: 1rem 0;
		}

		a {
			color: var(--gray-400);
			text-decoration: none;
			transition: color 0.24s;

			&:focus,
			&:hover {
				color: var(--gray-600);
			}
		}

		img {
			height: 1.25rem;
			width: auto;
			vertical-align: middle;
			margin: 0 0.25rem;
			display: inline-block;
		}
	}
</style>

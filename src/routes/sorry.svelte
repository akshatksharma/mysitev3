<script lang="ts">
	import Nav from '../components/Nav.svelte';
	import Page from '../components/Page.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<Page>
	<Nav />

	<div class="body">
		<h1 class="title">This page is still under construction.</h1>
		<p>Thanks for checking it out &lt;3</p>
	</div>
</Page>

<style>
	:global(*),
	:global(*::before),
	:global(*::after) {
		box-sizing: border-box;
	}

	:global(html),
	:global(body),
	:global(h1),
	:global(h2),
	:global(h3),
	:global(p) {
		margin: 0;
		padding: 0;
		border: 0;
		font-weight: 400;
	}

	.body {
		margin-top: 6rem;
		margin-bottom: 3rem;
	}

	.title {
		font-size: 2rem;
		margin-bottom: 1rem;
	}
</style>

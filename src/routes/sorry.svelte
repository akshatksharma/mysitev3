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
	.body {
		margin-top: 6rem;
		margin-bottom: 3rem;
	}

	.title {
		font-size: 2rem;
		margin-bottom: 1rem;
	}
</style>

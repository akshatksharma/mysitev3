<script lang="ts">
	import { Pages } from '../types';

	import Page from '../components/Page.svelte';
</script>

<Page currentPage={Pages.Travel}>
	<div class="body">
		<p class="sign">👷🏽</p>
		<h1 class="title">This page is still under construction.</h1>
		<p>Thanks for checking it out though &lt;3</p>
	</div>
</Page>

<style>
	.body {
		margin-top: 6rem;
		margin-bottom: 3rem;
	}

	.sign {
		font-size: 5rem;
	}

	.title {
		font-size: 2rem;
		margin-bottom: 1rem;
	}
</style>

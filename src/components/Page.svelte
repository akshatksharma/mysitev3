<script context="module">
	export const load = async ({ page }) => ({
		props: {
			key: page.path
		}
	});
</script>

<script lang="ts">
	import type { Pages } from '../types';
	import Nav from './Nav.svelte';
	import Transition from './Transition.svelte';

	export let key = undefined;
	export let currentPage: Pages = undefined;
</script>

<div class="page">
	<Nav {currentPage} />
	<Transition refresh={key}>
		<slot />
	</Transition>
</div>

<style>
	.page {
		height: 100vh;
		max-width: 700px;
		margin: 0 auto;
		padding: 1rem 2rem;
	}
</style>

<script lang="ts">
	import { Pages } from '../types';
	export let currentPage: Pages = undefined;
</script>

<nav>
	<a href=".">Akshat Sharma</a>
	<div class="group">
		{#each Object.keys(Pages) as page}
			<a class={Pages[page] == currentPage ? 'current' : ''} href="/{Pages[page]}">{page}</a>
		{/each}
	</div>
</nav>

<style>
	nav {
		display: flex;
		justify-content: space-between;
		margin-top: 2rem;
	}

	a {
		color: black;
		text-decoration: none;
	}

	a.current {
		font-weight: 700;
	}

	nav .group a {
		margin-left: 1rem;
	}
</style>

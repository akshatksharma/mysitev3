<script lang="ts">
	import { Pages } from '../types';
	export let currentPage: Pages = undefined;
</script>

<nav>
	<a class="home" href=".">Home</a>
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
		transition: color 300ms;
	}

	a.current {
		font-weight: 700;
	}

	nav .group a {
		display: inline-block;
		text-align: center;
		width: 4rem;
	}

	nav .group :not(a.current):hover,
	a.home:hover {
		color: #838181;
	}
</style>

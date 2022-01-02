<script>
	import { fly } from 'svelte/transition';
	export let refresh = '';
</script>

{#key refresh}
	<div in:fly={{ x: -2, duration: 400, delay: 400 }} out:fly={{ x: 2, duration: 400 }}>
		<slot />
	</div>
{/key}

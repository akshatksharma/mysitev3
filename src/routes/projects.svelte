<script lang="ts">
	import Nav from '../components/Nav.svelte';
	import Page from '../components/Page.svelte';
	import Footer from '../components/Footer.svelte';
	import { Pages } from '../types';
</script>

<Page>
	<Nav currentPage={Pages.Projects} />
	<Footer />
</Page>

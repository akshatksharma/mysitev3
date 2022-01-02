<script>
	// @ts-ignore
	import Typewriter from 'svelte-typewriter';
	import Nav from '../components/Nav.svelte';
	import Page from '../components/Page.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<svelte:head>
	<title>Akshat Sharma</title>
</svelte:head>

<Page>
	<div class="body">
		<div class="wavy" />
		<div class="titles">
			<Typewriter loop={5000} interval={[90, 100, 130]}>
				<h1 class="title">Hi, I'm Akshat</h1>
				<h1 class="title">नमस्ते, मैं अक्षत हूँ</h1>
			</Typewriter>
		</div>
		<p class="text">A fullstack developer based out of Dallas and St. Louis.</p>
		<p class="text">
			I love museums, photography, keyboards, korean fried chicken, and traveling. I’m currently
			working on finishing my degree in one piece, and not embarassing myself during pickup
			basketball games.
		</p>
	</div>
	<Footer />
</Page>

<style>
	.body {
		margin-top: 3rem;
		margin-bottom: 3rem;
	}

	.titles {
		height: 3rem;
		margin-bottom: 1rem;
	}

	.title {
		font-size: 2rem;
		font-weight: 500;
	}

	.text {
		margin-bottom: 0.5rem;
	}

	.wavy {
		margin-top: 3rem;
		margin-bottom: 3rem;
		width: 100%;
		height: 150px;
		background: linear-gradient(270deg, #fbd9cf, #f9d3e1, #c4e4f0, #bdece1);
		background-size: 800% 800%;

		animation: AnimationName 30s ease infinite;
	}

	@keyframes AnimationName {
		0% {
			background-position: 0% 50%;
		}
		50% {
			background-position: 100% 50%;
		}
		100% {
			background-position: 0% 50%;
		}
	}
</style>

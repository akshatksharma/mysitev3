<script lang="ts">
	import Footer from '../components/Footer.svelte';
	import Page from '../components/Page.svelte';
	import { Pages } from '../types';
</script>

<Page currentPage={Pages.Projects}>
	<div class="body">
		<div class="wavy" />
		<div class="list">
			<div class="projectBox">
				<!-- <img src="" alt="" class="image" /> -->
				<div class="content">
					<div class="header">
						<h2>
							<a href="https://mazeviz.netlify.app/	">MazeViz</a>
						</h2>
						<p>May 2020</p>
					</div>
					<p class="description">
						Mazeviz is a project I made to become more comfortable with vanilla JavaScript, graph
						search algorithms, and data visualization. I enjoy learning with visuals, so I wanted to
						make concepts in class come to life in an easy to use and informative site.
					</p>
				</div>
			</div>
			<div class="projectBox">
				<!-- <img src="" alt="" class="image" /> -->
				<div class="content">
					<div class="header">
						<h2><a href="https://grounded-archive-frontend.netlify.app/">Grounded</a></h2>
						<p>June 2020</p>
					</div>
					<p class="description">
						Grounded: The Pandemic Archive is a project that serves to take a snapshot of the
						COVID-19 pandemic. Users are encouraged share how they have found new meaning in the
						physical spaces and objects around them while in quanatine. Each submission consists of
						an image and a story, which can be recorded or typed. Built in collaboration with Design
						for America, I led the site's frontend work.
					</p>
				</div>
			</div>
		</div>
	</div>
	<Footer />
</Page>

<style>
	.body {
		margin-bottom: 3rem;
	}
	.projectBox {
		margin-bottom: 2rem;
	}
	.projectBox h2 a {
		font-weight: 700;
		font-size: 1.25rem;
		text-decoration: none;
	}

	a:focus {
		border-bottom: 1px solid;
	}

	a:hover {
		border-bottom: 1px solid;
	}

	.projectBox .header {
		margin-bottom: 0.5rem;
	}

	.projectBox .description {
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
</style>

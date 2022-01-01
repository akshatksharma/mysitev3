<script lang="ts">
	import Nav from '../components/Nav.svelte';
	import Page from '../components/Page.svelte';
	import Footer from '../components/Footer.svelte';
	import { Pages } from '../types';
</script>

<Page>
	<Nav currentPage={Pages.Projects} />
	<div class="body">
		<div class="list">
			<div class="projectBox">
				<img src="" alt="" class="image" />
				<div class="content">
					<h2>MazeViz</h2>
					<p>05 / 2020</p>
					<p>
						Mazeviz is a project I made to become more comfortable with vanilla Javascript, Graph
						search algorithms, and visualization. I enjoy learning with visuals, so I wanted to make
						concepts in class come to life in an easy to use and informative site. As a TA for my
						school's data structures/algorithms class, I used this site to make these algorithms
						'click' for the students I teach as well.
					</p>
				</div>
			</div>
		</div>
	</div>
	<Footer />
</Page>

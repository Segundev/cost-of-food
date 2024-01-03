<script>
	import '../style.css';

	import Article from '../components/Article.svelte';
	import Header from '../components/Header.svelte';
</script>

<div class="page-wrapper">
	<Header />
	<main>
		<Article />
	</main>
</div>

<style>
	.page-wrapper {
		width: 95%;
		max-width: 750px;
		margin: 0 auto;
		overflow-x: hidden;
	}

	/* @media (min-width: 650px) {
		.page-wrapper {
			width: 50%;
		}
	} */
</style>

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
		max-width: 390px;
		margin: 0 auto;
	}

	@media (min-width: 650px) {
		.page-wrapper {
			max-width: 550px;
		}
	}
</style>

<script>
	import '../style.css';

	import Article from '../components/Article.svelte';
	import Header from '../components/Header.svelte';
	import Footer from '../components/Footer.svelte';
	import Navbar from '../components/Navbar.svelte';
</script>

<div class="page-wrapper">
	<Navbar />
	<div class="main-wrapper">
		<Header />
		<main>
			<Article />
		</main>
	</div>
	<Footer />
</div>

<style>
	.main-wrapper {
		width: 98%;
		max-width: 850px;
		margin: 0 auto;
		overflow-x: hidden;
	}

	/* @media (min-width: 650px) {
		.page-wrapper {
			width: 50%;
		}
	} */
</style>

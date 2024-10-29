<script>
	import '../style.css';

	import Article from '../components/Article.svelte';
	import Header from '../components/Header.svelte';
	import Footer from '../components/Footer.svelte';
	import Navbar from '../components/Navbar.svelte';

	import Scrolly from '../lib/Scrolly.svelte';
	let currentStep;

	const steps = [
		'<p>In 2023, voter participation among the southern and southern-eastern states decreased significantly. Bayelsa State recorded its lowest percentage compared to the previous presidential elections of 2015 and 2019.</p>',
		'<p>In 2019, the decline right from 2007 was obvious in Enugu, Cross River, Rivers, Akwa Ibom, and other neighboring southern states. Most of these states recorded turnout above 40% in 2015 but declined to an average below 25% in 2019.</p>',
		'<p>Despite the fact that the voter turnout rate was above 40%, which means that at most 5 in 10 Nigerians voted, Lagos did horribly and had a lower turnout than Borno State, at a time when terrorism in the state was at its worst.</p>'
	];
</script>

<div class="page-wrapper">
	<Navbar />
	<Header />
	<div class="main-wrapper">
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
	}

	/* @media (min-width: 650px) {
		.page-wrapper {
			width: 50%;
		}
	} */
</style>

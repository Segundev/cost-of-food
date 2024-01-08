<script>
	export let chartName = '';
	export let altText = '';
</script>

<figure>
	<img src="/CHARTS/{chartName}" alt={altText} class="responsive" />
	<figcaption><slot /></figcaption>
</figure>

<style>
	figure {
		margin: 0;
		text-align: center;
	}

	img.responsive {
		max-width: 100%;
		width: 100%;
		height: auto;
	}

	figcaption {
		font-size: 12px;
		margin-top: -1.2rem;
		color: #ddf3d2;
	}

	@media (min-width: 550px) {
		img.responsive {
			width: 65%;
			max-width: 100%;
		}
	}
</style>

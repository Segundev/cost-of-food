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
		margin-left: 1.875rem;
		text-align: center;
	}

	img.responsive {
		max-width: 100%;
		width: 100%;
		height: auto;
	}

	figcaption {
		font-size: 12px;
		margin: -5px;
		color: #ddf3d2;
	}

	@media (min-width: 550px) {
		img.responsive {
			width: 100%;
			max-width: 100%;
		}
	}
</style>

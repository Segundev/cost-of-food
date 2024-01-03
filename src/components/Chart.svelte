<script>
	export let chartName = '';
	export let altText = '';
</script>

<figure>
	<img src="/CHARTS/{chartName}" alt={altText} />
	<figcaption><slot /></figcaption>
</figure>

<style>
	figure {
		margin: 0;
		margin-left: 1.875rem;
	}
	figcaption {
		padding-left: 15px;
		font-size: 12px;
		margin: -5px;
		color: #ddf3d2;
	}
</style>

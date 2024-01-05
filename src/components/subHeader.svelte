<script>
	export let id;
	export let fontSize = '1.2rem';
	export let borderBottom = 'none';
</script>

<div {id} class="subheading" style="border-bottom: {borderBottom};">
	<div class="circle">
		<div class="Ellipse"></div>
		<div
			style="left: 11px; top: 2px; position: absolute; color: white; font-size: 16px; font-family: Archivo; font-weight: 700; line-height: 29.60px; letter-spacing: 0.16px; word-wrap: break-word"
		>
			#
		</div>
	</div>
	<h2 class="text" style="font-size: {fontSize};"><slot /></h2>
</div>

<style>
	.subheading {
		height: 100%;
		display: flex;
		justify-content: flex-start;
		align-items: center;
		gap: 18px;
		margin-top: 1rem;
		margin-bottom: -1rem;
		margin-left: 1.875rem;
		margin-right: 1.875rem;
		padding-bottom: 8px;
	}

	.circle {
		width: 32px;
		height: 32px;
		position: relative;
	}

	.Ellipse {
		width: 32px;
		height: 32px;
		left: 0px;
		top: 0px;
		position: absolute;
		background: #b43b2b;
		border-radius: 9999px;
	}

	.text {
		font-weight: bold;
		word-wrap: break-word;
		margin: 0;
		color: var(--amber);
		line-height: 1.2;
	}
</style>

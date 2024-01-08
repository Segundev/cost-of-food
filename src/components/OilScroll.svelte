<script>
	import Scrolly from '../lib/Scrolly.svelte';
	import Chart from './Chart.svelte';
	import { chartData } from '../lib/chartType';

	let currentStep;
	let value = 3;

	const steps = [
		`Most recently, OPEC has cut Nigeria's oil production quota for 2024 by 20 percent, reducing it from 1.8 million barrels per day to 1.38 million barrels per day`,
		`The federal government has been unable to capitalize on the recent surge in petrol prices over the past year due to the expenses associated with subsidizing petrol. The oil price in June 2022 reached its highest level since 2014`
	];

	$: if (currentStep == 0) {
		value = 3;
	} else if (currentStep == 1) {
		value = 4;
	}
</script>

<div class="section-container">
	<div class="steps-container">
		<Scrolly bind:value={currentStep}>
			{#each steps as text, i}
				<div class="step" class:active={currentStep === i}>
					<div class="step-content"><p class="text">{text}</p></div>
				</div>
			{/each}
		</Scrolly>
	</div>
	<div class="sticky">
		<Chart chartName={chartData[value].chartName} altText={chartData[value].altText}></Chart>
	</div>
</div>

<style>
	.sticky {
		position: sticky;
		top: 25%;
		margin: auto;
		width: 90%;
		height: 100dvh;
	}

	.section-container {
		margin-top: 1em;
		text-align: center;
		transition: background 100ms;
		display: flex;
		flex-direction: column-reverse;
	}

	.step {
		height: 80vh;
		display: flex;
		place-items: center;
		justify-content: center;
	}

	.step-content {
		font-size: 14px;
		background: #283423;
		color: white;
		border: 1px #ffdd64 solid;
		padding: 0.5rem 0.5rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
		transition: background 500ms ease;
		box-shadow: 4px 5px 4px #0d110a;
		text-align: left;
		width: 75%;
		margin: auto;
		max-width: 375px;
		opacity: 0.7;
	}

	.text {
		margin: 0.75rem 0.75rem;
		font-size: 14px;
	}

	.step.active .step-content {
		background: #222b1e;
		color: white;
		opacity: 1;
	}

	.steps-container,
	.sticky {
		height: 100%;
	}

	.steps-container {
		flex: 1 1 40%;
		z-index: 10;
	}
</style>

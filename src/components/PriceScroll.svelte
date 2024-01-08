<script>
	import Scrolly from '../lib/Scrolly.svelte';
	import Chart from './Chart.svelte';
	import { chartData } from '../lib/chartType';

	let currentStep;
	let value = 2;

	const steps = [
		`Diesel is not subsidized, unlike petrol. The price of diesel rose from 200 naira in November 2022 and is currently being sold for over 1000 naira.`,
		`In August 2023, the Federal Government spent over 160 billion on subsidies. This was aimed at mitigating the impact of the removal, as prices rose from 200 naira to over 750 naira in some parts of the country.`,
		`The recurrent scarcity of fuel, coupled with the ultimate removal, has caused the price to surge from 165 naira since the Jonathan administration to over 750 naira in some parts of the country.`
	];

	$: if (currentStep == 0) {
		value = 2;
	} else if (currentStep == 1) {
		value = 8;
	} else if (currentStep == 2) {
		value = 6;
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
		<div class="spacer"></div>
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
	}

	.text {
		margin: 0.75rem 0.75rem;
		font-size: 14px;
	}

	.step.active .step-content {
		background: #222b1e;
		color: white;
	}

	.steps-container,
	.sticky {
		height: 100%;
	}

	.steps-container {
		flex: 1 1 40%;
		z-index: 10;
	}

	.spacer {
		margin-bottom: 80px;
	}
</style>

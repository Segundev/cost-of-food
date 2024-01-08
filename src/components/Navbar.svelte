<script>
	import Menu from '../lib/Icons/Menu.svelte';
	import Close from '../lib/Icons/Close.svelte';
	import MenuInner from './MenuInner.svelte';

	import { slide } from 'svelte/transition';
	import { quintOut } from 'svelte/easing';

	let isNavShowing = false;
</script>

<svelte:head>
	{#if isNavShowing}
		<style>
			body {
				overflow: hidden;
			}
		</style>
	{/if}
</svelte:head>

<nav>
	<div class="nav-wrapper">
		<a href="/">Orodata</a>
		<div class="icons">
			{#if !isNavShowing}
				<button on:click={() => (isNavShowing = !isNavShowing)}><Menu /></button>
			{:else}
				<div
					transition:slide={{ delay: 250, duration: 1000, easing: quintOut, axis: 'x' }}
					class="modal"
				>
					<div>
						<div class="close-button">
							<button on:click={() => (isNavShowing = !isNavShowing)}><Close /></button>
						</div>
						<MenuInner />
					</div>
				</div>
			{/if}
		</div>
	</div>
</nav>

<style>
	nav {
		position: fixed;
		top: 0;
		width: 100%;
		background: #fffbf5;
		height: 2.875rem;
		border-bottom: 4px solid #dea755;
		z-index: 9999;
	}

	.nav-wrapper {
		display: flex;
		justify-content: space-between;
		padding: 0 1.5rem;
	}

	.icons {
		padding-top: 4px;
	}

	.modal {
		position: fixed;
		right: 0%;
		background: #1c3013;
		border-left: 4px solid #dea755;
		top: -10px;
		z-index: 10;
	}

	.modal > div {
		margin: 1rem;
	}

	a {
		background-image: url('orodata-nav-logo.png');
		background-position: 95% 75%;
		padding-right: 2rem;
		text-transform: uppercase;
		letter-spacing: 0.05em;
		color: #484848;
		background-repeat: no-repeat;
		background-size: auto 70%;
		display: flex;
		align-items: center;
		max-width: max-content;
		height: 100%;
		padding-top: 8px;
		font-size: 1.2rem;
		font-weight: bold;
		text-decoration: none;
		cursor: pointer;
	}

	.close-button button {
		float: right;
	}
</style>

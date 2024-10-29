<script>
	import Menu from '../lib/Icons/Menu.svelte';
	import Close from '../lib/Icons/Close.svelte';
	import MenuInner from './MenuInner.svelte';

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
		<div class="icons">
			<button on:click={() => (isNavShowing = !isNavShowing)}>
				{#if !isNavShowing}
					<Menu />
				{:else}
					<Close />
				{/if}
			</button>
		</div>
	</div>
</nav>

<!-- The aside menu -->
<aside class:active={isNavShowing}>
	<div class="modal-content">
		<div class="asideMenu">
			<MenuInner />
		</div>
	</div>
</aside>

<!-- Overlay -->
<div class="overlay" class:active={isNavShowing} on:click={() => (isNavShowing = false)} />

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
		justify-content: center;
		padding: 0 1.5rem;
	}

	.icons {
		padding-top: 4px;
	}

	/* Aside styles */
	aside {
		position: fixed;
		top: 0;
		right: -100%; /* Start off-screen */
		height: 100vh;
		width: 100%; /* Adjust width as needed */
		background: #1c3013;
		border-left: 4px solid #dea755;
		z-index: 10000;
		transition: right 0.3s ease-in-out; /* Smooth transition */

		@media (min-width: 650px) {
			width: 50%;
		}
	}

	aside.active {
		right: 0; /* Slide in */
	}

	.modal-content {
		padding: 1rem;
		height: 100%;
	}

	/* Overlay styles */
	.overlay {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background: rgba(0, 0, 0, 0.5);
		opacity: 0;
		visibility: hidden;
		transition: opacity 0.3s ease-in-out;
		z-index: 9999;
	}

	.overlay.active {
		opacity: 1;
		visibility: visible;
	}

	/* Button styles */
	button {
		background: none;
		border: none;
		cursor: pointer;
		padding: 0;
	}

	.asideMenu {
		height: 100%;
		/* overflow-y: auto; */
	}
</style>

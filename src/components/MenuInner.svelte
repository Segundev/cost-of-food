<script>
	import SubHeader from './subHeader.svelte';
</script>

<aside>
	<div class="inner-wrapper">
		<a href="#1"
			><SubHeader fontSize={'1.3rem'} borderBottom={'3px solid #FFD79B'}
				>Christmas is expensive</SubHeader
			></a
		>
		<a href="#2"
			><SubHeader fontSize={'1.3rem'} borderBottom={'3px solid #FFD79B'}
				>Cost of farming has increased</SubHeader
			></a
		>
		<a href="#3"
			><SubHeader fontSize={'1.3rem'} borderBottom={'3px solid #FFD79B'}
				>Diesel a major reason why food is expensive</SubHeader
			></a
		>
		<a href="#4"
			><SubHeader fontSize={'1.3rem'} borderBottom={'3px solid #FFD79B'}
				>Border Closure and Exchange Rate and its negative effect</SubHeader
			></a
		>
		<a href="#5"
			><SubHeader fontSize={'1.3rem'} borderBottom={'3px solid #FFD79B'}
				>Other foods items are expensive too</SubHeader
			></a
		>
		<a href="#6"
			><SubHeader fontSize={'1.3rem'} borderBottom={'3px solid #FFD79B'}
				>How would households cope?</SubHeader
			></a
		>
	</div>
</aside>

<style>
	aside {
		height: 100dvh;
		overflow: hidden;
	}
	.inner-wrapper {
		display: flex;
		flex-direction: column;
		justify-content: start;
		gap: 3rem;
	}

	a {
		text-decoration: none;
	}
</style>

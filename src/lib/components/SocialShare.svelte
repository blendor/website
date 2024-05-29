<script lang="ts">
	import Circle from './Circle.svelte';
	import Rect from './Rect.svelte';

	let selected = Circle;
</script>

<svelte:component this={selected} />

<button on:click={() => (selected = Rect)}> X/Twitter </button>
<button on:click={() => (selected = Circle)}> Make it circle </button>

<style>
	</style <style > :global(svg) {
		max-width: 400px;
		display: block;
	}
</style>

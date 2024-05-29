<script lang="ts">
	import Header from '../lib/components/Header.svelte';
	import Footer from '../lib/components/Footer.svelte';
	import '../app.css';
	import Analytics from '$lib/components/Analytics.svelte';
</script>

<Header />
<slot />
<Footer />

<style>
	@import '../app.css';
	@import '../grid.css';
	@import '../header.css';
	@import '../footer.css';
	/* your styles go here */
</style>

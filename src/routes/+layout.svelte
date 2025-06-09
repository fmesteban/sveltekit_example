<script>
	import Header from './Header.svelte';
	import { injectAnalytics } from '@vercel/analytics/sveltekit'
	import { injectSpeedInsights } from '@vercel/speed-insights/sveltekit';

	injectSpeedInsights();
	injectAnalytics();
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>
</div>

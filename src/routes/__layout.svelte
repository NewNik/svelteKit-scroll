<script>
	import { browser } from '$app/env';
	import { navigating } from '$app/stores';
	import { tick } from 'svelte';

    // FIX scrollTo //
	// const scrollTo = browser && window.scrollTo;
    
	// $: if ($navigating) {
	// 	if (browser) {
	// 		window.scrollTo = async (...args) => {
	// 			console.log('custom scrollTo');
	// 			await tick();
	// 			scrollTo(...args);
	// 		};
	// 	}
	// } else {
	// 	if (browser && scrollTo) {
	// 		window.scrollTo = scrollTo;
	// 	}
	// }

</script>

<slot />

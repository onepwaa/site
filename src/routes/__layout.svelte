<!-- 1. Assign current route's path to `key` prop -->
<script context="module">
	export const load = async ({ url }) => ({
		props: {
			key: url
		}
	});
</script>

<script>
	import PageTransition from '../components/PageTransition.svelte';
	export let key;
</script>

<main>
	<div class="flex flex-col min-h-screen overflow-x-hiddent">
		<div class="bg-blue-900 py-3 px-4 text-white font-bold flex items-center" id="event-banner">
			<h3 class="flex-grow">Join Us On 29th January for the What The Pwaa! Debate Tournament</h3>
			<h3 class="text-5xl close font-normal">+</h3>
		</div>
		<div class="bg-gray-900 py-4 px-4">
			<a href="/"> <img src="img/onepwaa-logo-black.png" class="h-10 cursor-pointer" alt="OnePwaa" /></a>
		</div>

		<PageTransition refresh={key}>
			<slot />
		</PageTransition>
	</div>
	<style>
		body{
			width: 100vw!important;
			overflow-x: hidden;
		}
	</style>
</main>

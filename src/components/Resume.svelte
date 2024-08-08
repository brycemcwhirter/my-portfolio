<script>
	import { onMount } from 'svelte';
	import ExperienceCard from './ExperienceCard.svelte';

	let isMobile = false;

	onMount(() => {
		const checkMobile = () => {
			const mobileMediaQuery = window.matchMedia('(max-width: 768px)');
			isMobile = mobileMediaQuery.matches;
		};

		// Check on mount
		checkMobile();

		// Add a resize event listener to handle screen size changes
		window.addEventListener('resize', checkMobile);

		return () => {
			window.removeEventListener('resize', checkMobile);
		};
	});
</script>

<div
	class="grid min-h-screen grid-cols-1 items-center justify-center space-y-5 border p-6 md:grid-cols-2 md:p-8"
>
	<div
		id="codingLanguages"
		class="grid grid-cols-4 items-center justify-items-center gap-3 gap-y-9"
	>
		{#if isMobile}
			<i class="fa-brands fa-linkedin-in fa-2x"></i>
			<i class="fa-brands fa-linkedin-in fa-2x"></i>
			<i class="fa-brands fa-linkedin-in fa-2x"></i>
			<i class="fa-brands fa-linkedin-in fa-2x"></i>
			<i class="fa-brands fa-linkedin-in fa-2x"></i>
			<i class="fa-brands fa-linkedin-in fa-2x"></i>
			<i class="fa-brands fa-linkedin-in fa-2x"></i>
			<i class="fa-brands fa-linkedin-in fa-2x"></i>
		{:else}
			<i class="fa-brands fa-linkedin-in fa-3x"></i>
			<i class="fa-brands fa-linkedin-in fa-3x"></i>
			<i class="fa-brands fa-linkedin-in fa-3x"></i>
			<i class="fa-brands fa-linkedin-in fa-3x"></i>
			<i class="fa-brands fa-linkedin-in fa-3x"></i>
			<i class="fa-brands fa-linkedin-in fa-3x"></i>
			<i class="fa-brands fa-linkedin-in fa-3x"></i>
			<i class="fa-brands fa-linkedin-in fa-3x"></i>
		{/if}
	</div>
	<div id="experience" class="m-auto grid-cols-1 items-center justify-center space-y-6 p-1 md:p-6">
		<!-- todo do you really need this header
		<h1 class="flex items-center justify-center py-7 text-2xl font-bold">Experience</h1> -->

		<ExperienceCard />
	</div>
</div>

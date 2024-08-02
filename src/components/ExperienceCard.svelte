<script>
	import { onMount } from 'svelte';

	let experiences = [];

	onMount(async () => {
		const response = await fetch('/data/experience.json');
		experiences = await response.json();
	});
</script>

<!-- todo Align Text to Center if on a small screen-->
{#each experiences as experience}
	<div class="gap-1 p-5 text-left md:p-10">
		<h2 class="text-md font-bold md:text-xl lg:text-2xl">
			{experience.title}
		</h2>

		<a href={experience.companyLink} target="_blank">
			<h4 class="pad-8 text-md font-medium italic hover:underline md:text-lg">
				{experience.company}
			</h4>
		</a>
		<p class="pad-1 text-xs font-medium italic lg:text-lg">{experience.dateRange}</p>

		<p class="text-xs font-light lg:text-base">{experience.description}</p>

		<!-- {#each experience.bulletPoints as bulletPoint}
			<p class="text-xs font-light lg:text-base">•{bulletPoint}</p>
		{/each} -->
	</div>
{/each}

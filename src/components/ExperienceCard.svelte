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
	<div class="gap-1 space-y-1 border">
		<h2 class="text-md font-bold md:text-xl">{experience.title}</h2>
		<a href={experience.companyLink} target="_blank">
			<p class="pad-1 text-sm font-medium italic hover:underline md:text-base">
				{experience.company}
			</p>
		</a>
		<p class="text-xs font-light">{experience.description}</p>

		{#each experience.bulletPoints as bulletPoint}
			<p class="text-xs font-light">•{bulletPoint}</p>
		{/each}
	</div>
{/each}

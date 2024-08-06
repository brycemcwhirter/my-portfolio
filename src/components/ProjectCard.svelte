<script>
	import { onMount } from 'svelte';

	let projects = [];

	onMount(async () => {
		const response = await fetch('/data/projects.json');
		projects = await response.json();
	});
</script>

{#each projects as project}
	<div class="mx-auto max-w-lg p-10">
		<div class="mb-5 max-w-sm rounded-lg border border-gray-800">
			<img class="rounded-t-lg" src={project.imgLink} alt="" />

			<div class="p-5">
				<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
					{project.title}
				</h5>

				<p class="mb-3 flex items-center justify-center font-normal text-gray-700 dark:text-white">
					{project.description}
				</p>
				<a
					class="flex items-center justify-center rounded-lg"
					href={project.githubLink}
					target="_blank"
				>
					<i class="fa-brands fa-github fa-2x"></i>
				</a>
			</div>
		</div>
	</div>
{/each}

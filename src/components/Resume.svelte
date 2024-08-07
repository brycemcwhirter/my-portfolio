<script>
	import ExperienceCard from './ExperienceCard.svelte';
</script>

<div class="grid min-h-screen grid-cols-1 space-y-5 p-6 md:p-8">
	<!-- <h1
		class="align-center flex items-center justify-center text-2xl font-bold md:text-3xl lg:hidden"
	>
		Experience
	</h1> -->
	<div class="grid grid-cols-1 gap-y-9 lg:grid-cols-2 lg:space-x-4">
		<div id="codingLanguages" class="m-auto grid grid-cols-1 items-center space-y-6 p-3">
			<h1 class="flex justify-center text-xl font-semibold md:text-2xl lg:text-3xl">
				Technology Skills
			</h1>
			<div
				class="grid grid-cols-4 items-center justify-items-center gap-x-14 gap-y-4 md:gap-x-28 md:gap-y-9"
			>
				<!--TODO svelte icon!-->
				<!-- Icons to show on small screens -->
				<i class="fa-brands fa-js fa-2x md:hidden"></i>
				<i class="fa-brands fa-php fa-2x md:hidden"></i>
				<i class="fa-brands fa-java fa-2x md:hidden"></i>
				<i class="fa-brands fa-python fa-2x md:hidden"></i>
				<!-- <i class="fa-brands fa-react fa-2x md:hidden"></i>
				<i class="fa-brands fa-vuejs fa-2x md:hidden"></i>
				<i class="fa-brands fa-tailwind fa-2x md:hidden"></i>
				<i class="fa-brands fa-docker fa-2x md:hidden"></i> -->

				<!-- Icons to show on medium screens -->
				<i class="fa-brands fa-js fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-php fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-java fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-python fa-3x hidden md:inline lg:hidden"></i>
				<!-- <i class="fa-brands fa-react fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-vuejs fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-vuejs fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-docker fa-3x hidden md:inline lg:hidden"></i> -->

				<!-- Icons to show on large screens -->
				<i class="fa-brands fa-js fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-php fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-java fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-python fa-5x hidden lg:inline"></i>
				<!-- <i class="fa-brands fa-react fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-vuejs fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-vuejs fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-docker fa-5x hidden lg:inline"></i> -->
			</div>
		</div>

		<div
			id="experience"
			class="m-auto grid-cols-1 items-center justify-center space-y-6 p-3 md:p-6"
		>
			<h1 class="align-center flex justify-center text-xl font-semibold md:text-2xl lg:text-3xl">
				Resumé
			</h1>

			<h2 class="align-center text-md flex justify-center font-medium md:text-xl lg:text-2xl">
				Education
			</h2>

			<div class="p-5 md:p-10">
				<p class="text-md font-bold md:text-xl lg:text-2xl">
					Bachelor of Science in Computer Science
				</p>
				<p class="text-md font-medium italic md:text-lg">Baylor University</p>
				<p class="pad-1 text-xs font-medium italic lg:text-lg">2023</p>
			</div>

			<h2 class="align-center flex justify-center text-lg font-medium md:text-xl lg:text-2xl">
				Professional Experience
			</h2>

			<ExperienceCard />
			<!--todo Download Resumé Button-->
			<div class="flex items-center justify-center">
				<a
					href="/Gene Bryce McWhirter Resume.pdf"
					class="border px-4 py-2 hover:bg-white hover:text-black"
					target="_blank">Download Resumé Here</a
				>
			</div>
		</div>
	</div>
</div>

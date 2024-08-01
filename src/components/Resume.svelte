<script>
	import ExperienceCard from './ExperienceCard.svelte';
</script>

<div class="grid min-h-screen grid-cols-1 space-y-5 border p-6 md:p-8">
	<!-- <h1
		class="align-center flex items-center justify-center text-2xl font-bold md:text-3xl lg:hidden"
	>
		Experience
	</h1> -->
	<div class="grid grid-cols-1 gap-y-9 lg:grid-cols-2 lg:space-x-4">
		<div id="codingLanguages" class="m-auto grid grid-cols-1 items-center space-y-6 p-3">
			<h1 class="flex justify-center text-xl font-semibold md:text-2xl lg:text-3xl">
				Coding Languages
			</h1>
			<div
				class="grid grid-cols-4 items-center justify-items-center gap-x-14 gap-y-4 md:gap-x-28 md:gap-y-9"
			>
				<!-- Icons to show on small screens -->
				<i class="fa-brands fa-linkedin-in fa-2x md:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-2x md:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-2x md:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-2x md:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-2x md:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-2x md:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-2x md:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-2x md:hidden"></i>

				<!-- Icons to show on medium screens -->
				<i class="fa-brands fa-linkedin-in fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-3x hidden md:inline lg:hidden"></i>
				<i class="fa-brands fa-linkedin-in fa-3x hidden md:inline lg:hidden"></i>

				<!-- Icons to show on large screens -->
				<i class="fa-brands fa-linkedin-in fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-linkedin-in fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-linkedin-in fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-linkedin-in fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-linkedin-in fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-linkedin-in fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-linkedin-in fa-5x hidden lg:inline"></i>
				<i class="fa-brands fa-linkedin-in fa-5x hidden lg:inline"></i>
			</div>
		</div>

		<div
			id="experience"
			class="m-auto grid-cols-1 items-center justify-center space-y-6 p-3 md:p-6"
		>
			<h1 class="align-center flex justify-center text-xl font-semibold md:text-2xl lg:text-3xl">
				Resumé
			</h1>
			<ExperienceCard />
		</div>
	</div>

	<!--todo Download Resumé Button-->
</div>

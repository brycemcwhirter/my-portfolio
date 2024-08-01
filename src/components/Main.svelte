<script>
	import Resume from './Resume.svelte';
	import Project from './Project.svelte';
</script>

<main class="dark:bg-black dark:text-white">
	<section id="introPage">
		<div class="flex min-h-screen flex-col items-center justify-center border">
			<h1 class="text-2xl font-semibold md:text-4xl">Bryce McWhirter</h1>
			<p class="text-lg font-medium md:text-2xl">Full Stack Developer</p>
			<p class="text-md font-medium md:text-lg">DFW</p>
		</div>
	</section>
	<section id="aboutPage">
		<div
			class="flex min-h-screen flex-col items-center justify-center space-y-10 border md:space-y-12"
		>
			<h1 class="text-2xl font-semibold md:text-3xl">About Me</h1>
			<p class="m-4 text-center md:m-28 lg:m-32">
				I'm a graduate from Baylor University with a Bachelor of Science in Computer Science and a
				minor in Entrepreneurship and Corporate Innovation. My programming experience began when I
				was a senior in high school, writing programs for a TI-84 calculator. Since then, I've
				gained extensive experience in multiple technologies by building various projects both in
				academia and during my free time. Keep scrolling to see my experience and the projects I've
				worked on and am currently working on.
			</p>
		</div>
	</section>

	<section id="resumePage">
		<Resume />
	</section>
	<section id="projectPage">
		<Project />
	</section>
	<section id="contactPage">
		<div class="flex min-h-screen flex-col items-center justify-center space-y-6 border sm:p-px">
			<h1 class="text-2xl font-semibold lg:text-4xl">Contact</h1>
			<p class="text-md m-4 text-center lg:m-32 lg:text-lg">Feel free to reach out.</p>
			<div class="flex-row space-x-5">
				<a
					href="https://www.linkedin.com/in/bryce-mcwhirter-5b9330146/"
					target="_blank"
					rel="noopener noreferrer"
				>
					<i class="fa-brands fa-linkedin-in fa-xl"></i>
				</a>
				<a href="https://github.com/brycemcwhirter" target="_blank" rel="noopener noreferrer">
					<i class="fa-brands fa-github fa-xl"></i>
				</a>
				<a href="mailto:mcwhirterbryce@gmail.com" target="_blank" rel="noopener noreferrer">
					<i class="fa fa-envelope fa-xl" aria-hidden="true"></i>
				</a>
			</div>
		</div>
	</section>
</main>

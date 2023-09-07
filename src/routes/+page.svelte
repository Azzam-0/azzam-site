<script>
	import Linkedin from '$lib/icons/Linkedin.svelte';
	import Tiktok from '$lib/icons/Tiktok.svelte';

	let bullets = [
		'Website Design.',
		'Mobile App Design.',
		'Graphic Design.'
	];
</script>

<div class="grid justify-center items-center pt-10">
	<div
		class="flex flex-col-reverse xl:flex-row border-2 border-[#281f15] p-10 justify-between xl:gap-32 gap-10 mx-8 mb-8 rounded-2xl"
	>
		<div class="flex flex-col justify-between xl:gap-0 gap-8">
			<div class="flex flex-col gap-8 max-w-2xl">
				<h1 class="xl:text-8xl text-3xl font-semibold font-poppins text-[#281f15]">Azzam Safar</h1>
				<h2 class="xl:text-2xl text-xl font-normal font-poppins text-[#281f15]">
					Hi there! I'm a designer with over 4 years of hands-on experience, working with projects
					from all over the world and I love creating unforgettable user experiences, Let's connect and work on something awesome
					together!
				</h2>
				<div class="flex flex-col gap-4">
					<h3 class="xl:text-2xl text-xl font-semibold font-poppins text-[#281f15]">
						What I Do
					</h3>
					<ul class="list-disc font-poppins text-[#281f15] xl:text-lg text-md flex flex-col gap-2">
						{#each bullets as bullet}
						<li>{bullet}</li>
						{/each}
					</ul>
				</div>
			</div>
			<div class="flex gap-4">
				<a target="_blank" rel="noopener noreferrer" href="https://www.tiktok.com/@azzam.safar">
					<Tiktok />
				</a>
				<a
					target="_blank"
					rel="noopener noreferrer"
					href="https://www.linkedin.com/in/azzam-safar/"
				>
					<Linkedin />
				</a>
			</div>
		</div>
		<img src="/images/azzam.webp" alt="Azzam Safar's face" class="mx-auto max-h-[40rem] rounded-2xl" />
	</div>
</div>

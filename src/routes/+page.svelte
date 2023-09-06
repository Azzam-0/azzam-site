<script>
	import Linkedin from '$lib/icons/Linkedin.svelte';
	import Tiktok from '$lib/icons/Tiktok.svelte';
</script>

<div class="grid justify-center items-center">
	<div
		class="flex flex-col-reverse lg:flex-row border-2 border-[#281f15] p-10 justify-between lg:gap-32 gap-10 mx-8 mb-8"
	>
		<div class="flex flex-col justify-between lg:gap-0 gap-8">
			<div class="flex flex-col gap-4 max-w-2xl">
				<h1 class="lg:text-8xl text-3xl font-semibold font-poppins text-[#281f15]">Azzam Safar</h1>
				<h2 class="lg:text-2xl text-xl font-light font-poppins text-[#281f15]">
					Hi there! I'm a designer with over 4 years of hands-on experience, working with projects
					from all over the world and I love creating unforgettable user experiences, I'm skilled in
					making websites, web apps, and mobile apps. Let's connect and work on something awesome
					together!
				</h2>
			</div>
			<div class="flex gap-4">
				<a href="https://www.tiktok.com/@azzam.safar">
					<Tiktok />
				</a>
				<a href="https://www.linkedin.com/in/azzam-safar/">
					<Linkedin />
				</a>
			</div>
		</div>
		<img src="/images/azzam.webp" alt="Azzam Safar's face" class="mx-auto max-h-[40rem]" />
	</div>
</div>

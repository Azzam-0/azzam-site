<script>
	let projects = [
		{
			title: 'Unideals',
			description: `Unideals is a student discount app that helps students save money on their favorite brands, I was responsible for creating the full user experience and user interface for the app, also created the full brand guidelines and brand identity, and much more!`,
			type: 'Mobile App',
			location: 'London, United Kingdom',
			languages: 'English, Arabic',
			bulletsTitle: 'What I Did',
			bullets: [
				'Created full user experience & user interface.',
				'Created full brand guidelines and brand identity.',
				'Created logo and graphic assets.'
			],
			link1: 'https://www.myunideals.com/',
			link2: 'https://www.linkedin.com/in/azzam-safar/details/recommendations/',
			image: '/images/app.webp'
		},
		{
			title: 'Macandsoft',
			description: `Macandsoft is an IT company that provides IT solutions for businesses, I was responsible for creating the full user experience and user interface for the website, also created the full brand guidelines and brand identity, and much more!`,
			type: 'Website',
			location: 'Berlin, Germany',
			languages: 'English, Spanish, German',
			bulletsTitle: 'What I Did',
			bullets: [
				'Created full user experience & user interface.',
				'Created full brand guidelines and brand identity.',
				'Created logo and graphic assets.'
			],
			link1: 'https://www.macandsoft.com/',
			link2: 'https://www.linkedin.com/in/azzam-safar/details/recommendations/',
			image: '/images/macandsoft.webp'
		},
		{
			title: 'Inosio',
			description: `Inosio is a property management software that helps property managers manage properties. I was responsible for creating the complete user experience and user interface for the web app. Additionally, I developed the entire brand guidelines and brand identity, among other responsibilities.`,
			type: 'SaaS',
			location: 'San Diego, United States',
			languages: 'English, Arabic, Spanish',
			bulletsTitle: 'What I Did',
			bullets: [
				'Created full user experience & user interface.',
				'Created full brand guidelines and brand identity.',
				'Created presentations, brochures, logo, and various graphic assets.'
			],
			link1: 'https://www.inosio.com/',
			link2: 'https://www.linkedin.com/in/azzam-safar/details/recommendations/',
			image: '/images/inosio.webp'
		}
	];
</script>

{#each projects as project, i}
	<section class="grid justify-center items-center pt-10">
		<div
			class={`flex flex-col-reverse border-2 border-[#281f15] rounded-2xl p-10 justify-between xl:gap-32 gap-10 mx-8 mb-8 ${
				i % 2 == 0 ? 'xl:flex-row' : 'xl:flex-row-reverse'
			}`}
		>
			<div class="flex flex-col justify-between xl:gap-0 gap-8">
				<div class="flex flex-col gap-8 max-w-2xl">
					<div class="flex flex-col gap-3">
						<h1 class="xl:text-8xl text-3xl font-semibold font-poppins text-[#281f15]">
							{project.title}
						</h1>
						<div class="flex gap-4 flex-wrap text-center">
							<h3
								class="bg-[#281f15] rounded-2xl :text-2xl text-md font-medium font-poppins text-white p-2 px-4"
							>
								{project.type}
							</h3>

							<h3
								class="bg-[#281f15] rounded-2xl :text-2xl text-md font-medium font-poppins text-white p-2 px-4"
							>
								{project.location}
							</h3>
							<h3
								class="bg-[#281f15] rounded-2xl :text-2xl text-md font-medium font-poppins text-white p-2 px-4"
							>
								{project.languages}
							</h3>
						</div>
					</div>
					<h2 class="xl:text-2xl text-xl font-normal font-poppins text-[#281f15]">
						{project.description}
					</h2>
					<div class="flex flex-col gap-4">
						<h3 class="xl:text-2xl text-xl font-semibold font-poppins text-[#281f15]">
							{project.bulletsTitle}
						</h3>
						<ul
							class="list-disc font-poppins text-[#281f15] xl:text-lg text-md flex flex-col gap-2"
						>
							{#each project.bullets as bullets}
								<li>{bullets}</li>
							{/each}
						</ul>
					</div>
				</div>
				<div class="flex gap-4 md:flex-row flex-col text-center">
					<a
						class="bg-transparent hover:bg-[#281f15] text-[#281f15] hover:text-white border-2 border-[#281f15] rounded-2xl hover:border-transparent font-poppins font-semibold text-xl p-4 w-full"
						href={project.link1}
						target="_blank"
						rel="noopener noreferrer"
					>
						Live Project
					</a>
					<a
						class="bg-transparent hover:bg-[#281f15] text-[#281f15] hover:text-white border-2 border-[#281f15] rounded-2xl hover:border-transparent font-poppins font-semibold text-xl p-4 w-full"
						href={project.link2}
						target="_blank"
						rel="noopener noreferrer"
					>
						Customer Review
					</a>
				</div>
			</div>
			<img src={project.image} alt={project.title} class="mx-auto max-h-[40rem]" />
		</div>
	</section>
{/each}

<script>
	import Linkedin from '$lib/icons/Linkedin.svelte';
	import Tiktok from '$lib/icons/Tiktok.svelte';
	import { onMount } from 'svelte';

  let sections = [
    {
      name: 'Azzam Safar',
      description: 'Hi there! I\'m a designer with over 4 years of hands-on experience, working with projects from all over the world and I love creating unforgettable user experiences, I\'m skilled in making websites, web apps, and mobile apps. Let\'s connect and work on something awesome together!',
      imageSrc: '/images/azzam.webp',
      socialLinks: [
        { href: 'https://www.tiktok.com/@azzam.safar', icon: 'Tiktok' },
        { href: 'https://www.linkedin.com/in/azzam-safar/', icon: 'Linkedin' }
      ]
    },
    // Add more sections here...
  ];

  onMount(() => {
    // Any additional initialization logic
  });
  export let section: {
    name: string;
    description: string;
    imageSrc: string;
    socialLinks: { href: string; icon: string }[];
  };
  </script>

<div class="grid justify-center items-center">
	{#each sections as section}
	  <Section {section} />
	{/each}
  </div>
  
  <div class="flex flex-col-reverse lg:flex-row border-2 border-[#281f15] p-10 justify-between lg:gap-20 gap-10 mx-8 mb-8">
	<div class="flex flex-col justify-between lg:gap-0 gap-8">
	  <div class="flex flex-col gap-4 max-w-2xl">
		<h1 class="lg:text-8xl text-3xl font-semibold font-poppins text-[#281f15]">{section.name}</h1>
		<h2 class="lg:text-2xl text-xl font-light font-poppins text-[#281f15]">{section.description}</h2>
	  </div>
	  <div class="flex gap-4">
		{#each section.socialLinks as link}
		  <a href={link.href}>
		  </a>
		{/each}
	  </div>
	</div>
	<img src={section.imageSrc} alt="{section.name}'s face" class="mx-auto max-h-[40rem]" />
  </div>
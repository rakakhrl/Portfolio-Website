<script>
	export let segment;

	const pages = [
		{
			'name': 'Home',
			'path': '.',
			'segment': undefined
		},
		{
			'name': 'Projects',
			'path': 'projects',
			'segment': 'projects'
		},
		{
			'name': 'Skills',
			'path': 'skills',
			'segment': 'skills'
		},
		{
			'name': 'Contact Me',
			'path': 'contact',
			'segment': 'contact'
		}
	];
</script>

<nav class="bg-white h-screen w-1/3 p-20">
	{#each pages as page}
		<div 
			class:bg-green={segment === page.segment} 
			class:text-white={segment === page.segment} 
			class:text-black={segment != page.segment} 
			class:pr-4={segment === page.segment} 
			class="p-0 mb-6"
		>
			<a 
				class='block text-4xl text-right font-viga' 
				href={page.path}
			>
				{page.name}
			</a>
		</div>
	{/each}
</nav>
<script>
	import { fly } from 'svelte/transition';
	import { onMount } from 'svelte';

	let show = false;

	onMount(() => {
		show = true;
	});
</script>

<svelte:head>
	<title>Sapper project template</title>
</svelte:head>


<div class="bg-black">
	<img src="coding-bg.png" alt="" class="relative h-screen object-cover opacity-25"/>

	<div class="absolute top-0 left-0 h-screen pt-32 p-20">
		{#if show}
			<p class="font-viga text-white text-6xl items-center" in:fly="{{x: -600, duration: 800}}">Hi, <br/> I'm Raka Khairil <br/> and <br/> I'm a frontend developer.</p>
		{/if}
	</div>
</div>


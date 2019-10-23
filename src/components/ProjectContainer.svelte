<script>
    import { fly } from 'svelte/transition';

    export let imgSrc;
    export let name;
    export let description;
    export let projectLink;
    export let codeLink;
    export let index;
</script>

<div class="flex w-full bg-white shadow-lg mb-8" in:fly="{{x: -1000, duration: 1000 + (400 * index)}}">
    <img src="coding-bg.png" alt="image" class="w-1/4 object-cover"/>
    <div class="px-8 py-4 w-1/2">
        <p class="font-viga text-3xl text-black">Project Name</p>
        <p class="text-md text-black font-roboto">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    </div>
    <div class="px-8 py-4 w-1/4">
        <button class="bg-green w-full h-12 text-white font-viga text-lg">Open</button>
        <div class="h-2"></div>
        <button class="w-full h-12 text-orange font-viga text-lg">Code</button>
    </div>
</div>
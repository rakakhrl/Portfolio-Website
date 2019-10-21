<script>
    import { fade, fly } from 'svelte/transition';

    let logos = ['nodejs', 'git-scm', 'firebase', 'flutterio', 'svelte', 'reactjs', 'tailwindcss', 'figma'];
</script>

<div class="flex flex-wrap pt-32 p-20">
    {#each logos as logo, i}
        <img src="logo/{logo}-icon.svg" alt="{logo} logo" in:fade={{duration: 1000 + (i * 200) }} class="h-1/5 w-1/5 mb-12 mr-8 block"/>
    {/each}
</div>
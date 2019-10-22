<script>
    import ProjectContainer from '../components/ProjectContainer.svelte';
</script>

<div class="p-20 max-h-screen overflow-scroll">
    <div class="bg-white w-full h-16 mb-8 shadow-lg">
        a
    </div>
    {#each [1,2,3,4,5,6] as p,i}
        <ProjectContainer/>
    {/each}
</div>

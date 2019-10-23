<script>
	import ProjectContainer from '../components/ProjectContainer.svelte';
	import ProjectToolbar from '../components/ProjectToolbar.svelte';
</script>

<div class="p-20 max-h-screen overflow-scroll">
	<ProjectToolbar/>
	{#each [1,2,3,4,5,6] as p,i}
		<ProjectContainer index={i}/>
	{/each}
</div>


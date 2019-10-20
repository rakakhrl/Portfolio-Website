<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<div class="flex">
	<main class="w-2/3 bg-grey">
		<slot></slot>
	</main>
	
	<Nav {segment}/>
</div>
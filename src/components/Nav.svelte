<script>
	export let segment;

	$: homeSegment = segment === undefined;
</script>

<nav class="bg-white h-screen w-1/3 p-20">
	<div class:bg-green={homeSegment} class:text-white={homeSegment} class:text-black={!homeSegment} class:pr-4={homeSegment} class="p-0 mb-6">
		<a class='block text-4xl text-right font-viga' href='.'>Home</a>
	</div>
</nav>
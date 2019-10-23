<script>
	let textField;
</script>

<div class="bg-white w-full h-16 mb-8 shadow-lg py-4 px-8">
	<input 
		type="text" 
		class="bg-white focus:outline-none border-b-2 border-grey focus:border-green py-1 px-2 font-roboto text-green" 
		placeholder="Search project name..."
		bind:value={textField}
	>
	<button 
		class="w-24 h-8 text-white font-viga text-md shadow-md ml-4"
		class:bg-green={textField != undefined}
		class:bg-grey={textField === "" || textField === undefined}
	>
		Search
	</button>
	{textField}
</div>
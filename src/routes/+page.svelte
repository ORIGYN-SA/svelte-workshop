<script lang="ts">
	import { counter } from '../store';
	function increment() {
		counter.update((n) => n + 1);
	}

	// Items for loop
	let fruits = [
		{ id: 1, name: 'apple' },
		{ id: 2, name: 'banana' },
		{ id: 3, name: 'strawberry' },
		{ id: 4, name: 'kiwi' },
		{ id: 5, name: 'tangerine' }
	];
</script>

<h1 class="my-8 text-3xl">Welcome to SvelteKit</h1>

<h1 class="text-xl font-bold text-orange-600">Hello world from Origyn!</h1>

<p class="my-4">The count is : {$counter}</p>

<button
	on:click={increment}
	class=" my-8 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
>
	add one</button
>

<h3 class="text-lg my-8 font-bold">Let's loop</h3>

{#each fruits as fruit}
	<p>{fruit.name}</p>
{/each}

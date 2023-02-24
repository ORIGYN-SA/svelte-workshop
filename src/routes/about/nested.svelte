<script lang="ts">
	import { counter } from '../../store';

	function increment() {
		counter.update((n) => n + 1);
	}
</script>

<p>This is my nested super useful component</p>

<p class="my-4">{$counter}</p>

<button
	on:click={increment}
	class=" my-8 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
>
	add one</button
>

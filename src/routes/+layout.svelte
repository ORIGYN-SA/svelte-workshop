<script>
	import '../app.css';
	import { counter } from '../store';

	let counterValue;

	counter.subscribe((value) => {
		counterValue = value;
	});
</script>

<div class="container my-12 mx-auto">
	<nav class="text-blue-500 font-bold">
		<a href="/">Home</a>
		<a href="/about">About</a>
		<a href="/profile">Profile</a>
		<a href="/blog">Blog</a>
	</nav>
	<div class="my-16">
		<slot />
	</div>
</div>

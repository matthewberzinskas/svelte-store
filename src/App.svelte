<script>
	import { count } from './stores.js';
	import Incrementer from './components/Incrementer.svelte';
	import Decrementer from './components/Decrementer.svelte';
	import Resetter from './components/Resetter.svelte';

	let countValue;

	count.subscribe(value => {
		countValue = value;
	});
</script>

<h1>The count is {countValue}</h1>

<div class="container">
	<Incrementer/>
	<Decrementer/>
	<Resetter/>
</div>

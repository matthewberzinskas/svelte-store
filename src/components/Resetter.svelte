<script>
	import { count } from '../stores.js';

	function reset() {
		count.update(n => n = 0);
	}
</script>

<button on:click={reset}>
	reset
</button>
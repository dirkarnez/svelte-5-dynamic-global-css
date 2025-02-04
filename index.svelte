<script>
	import Nested from './Nested.svelte';
	let count = $state(1);

	function handleClick() {
		count += 1;
	}
</script>

<button onclick={handleClick}>
	Count: {count}
</button>

<h1>123242</h1>

<p>These styles...</p>
{#if count % 2 == 0}
	<Nested />
{/if}

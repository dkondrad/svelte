<script>
	export let thePromise;
</script>

{#await thePromise}
	<p>loading...</p>
{:then theValue}
	<p>the value is {theValue}</p>
{:catch theError}
	<p>oh no! {theError.message}</p>
{/await}

{#await thePromise}
	<p>loading...</p>
{:then theValue}
	<p>the value is {theValue}</p>
{:catch theError}
	<p>oh no! {theError.message}</p>
{/await}
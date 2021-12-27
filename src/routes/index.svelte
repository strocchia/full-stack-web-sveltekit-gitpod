<script>
	import Item from '$lib/item.svelte';

	const title = 'New | Todos are phun';
</script>

<svelte:head>
	<title>{title}</title>
</svelte:head>

<div class="todos">
	<h1>{title}</h1>

	<form class="new" action="" method="">
		<input type="text" name="text" aria-label="Add todo" placeholder="Add a todo" />
	</form>

	<Item />
	<Item />
</div>

<style>
	.todos {
		width: 100%;
		max-width: 42rem;
		margin: 0 auto;
		margin-top: 4rem;
	}

	.new {
		margin-bottom: 1rem;
	}

	.new input {
		font-size: 28px;
		width: 100%;
		padding: 0.25em;
		box-sizing: border-box;
		background-size: rgba(255, 255, 255, 0.05);
		border-radius: 8px;
		text-align: center;
	}

	.todos :global(input) {
		border: 1px solid transparent;
	}
</style>

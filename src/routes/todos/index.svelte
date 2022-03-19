<script context="module">
	export async function load({ fetch }) {
		const res = await fetch('https://jsonplaceholder.typicode.com/todos');
		const todos = await res.json();

		if (res.ok) {
			return {
				props: {
					todos
				}
			};
		}

		return {
			status: res.status,
			error: new Error('Could not fetch the data')
		};
	}
</script>

<script>
	export let todos;
</script>

<div id="background" src="" alt="" />

{#each todos as todo}
	<div>
		<a href={`todos/${todo.id}`}>{todo.title}</a>
	</div>
{/each}

<style>
	div {
		margin: 1rem;
	}

	#background {
		margin: 0rem;
		width: 100%;
		height: 100vh;
		position: absolute;
		border: none;
		background-image: url('./background.png');
		background-position: center;
		background-size: cover;
		z-index: -1;
		top: 0;
		left: 0;
	}
</style>

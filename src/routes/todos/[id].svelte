<script context="module">
	export async function load({ fetch, params }) {
		const id = params.id;
		const res = await fetch(`https://jsonplaceholder.typicode.com/todos/${id}`);
		const todo = await res.json();

		if (res.ok) {
			return {
				props: {
					todo
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
	export let todo;
</script>

<h1>Title: {todo.title}</h1>
<p>cool</p>

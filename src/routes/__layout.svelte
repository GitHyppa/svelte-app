<script lang="ts">
	import '../app.css';
</script>

<header>
	<h1>HEADER</h1>
</header>

<main>
	<slot />
</main>

<footer>
	<h1>FOOTER</h1>
</footer>

<style>
	header {
		text-align: center;
	}

	footer {
		text-align: center;
	}
</style>

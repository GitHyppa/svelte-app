<script lang="ts">
	import Header from '../components/Header.svelte';

	import '../app.css';
	import Footer from '../components/Footer.svelte';
</script>

<Header />

<main>
	<slot />
</main>

<Footer />
